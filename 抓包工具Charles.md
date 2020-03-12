### 直接用Charles抓包工具抓Flutter APP 是抓不到http请求的，需要先设置代理

#### Dio
```
import 'package:dio/adapter.dart';
Dio dio=new Dio();
  // 代理
(dio.httpClientAdapter as DefaultHttpClientAdapter).onHttpClientCreate = (client) {
  // config the http client
  client.findProxy = (uri) {
      //proxy all request to localhost:8888
      return "PROXY 192.168.1.142:8888";
  };
  // you can also create a new HttpClient to dio
  // return new HttpClient();
};
```
### HttpClient
```
HttpClient client = HttpClient();
client.findProxy = (uri) {
  // 用1个开关设置是否开启代理
  return AppConstant.isDebug ?  "PROXY 192.168.5.5:8888" : 'DIRECT';
};
```
