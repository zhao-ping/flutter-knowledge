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

### 真机调试
1. 将手机网络与电脑网络设置成一致的
2. 设置手机网络代理：配置代理（HTTP代理）-> 选择手动代理 -> 设置服务器地址与电脑一致 -> 设置端口为 8888
