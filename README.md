# flutter-knowledge
flutter 运用的一些小知识

## ios权限
位置：**/ios/Flutter/App.framework/Info.plist

```
<!-- 相册 -->   
<key>NSPhotoLibraryUsageDescription</key>   
<string>App需要您的同意,才能访问相册</string>   
<!-- 相机 -->   
<key>NSCameraUsageDescription</key>   
<string>App需要您的同意,才能访问相机</string>   
<!-- 麦克风 -->   
<key>NSMicrophoneUsageDescription</key>   
<string>App需要您的同意,才能访问麦克风</string>   
<!-- 位置 -->   
<key>NSLocationUsageDescription</key>   
<string>App需要您的同意,才能访问位置</string>   
<!-- 在使用期间访问位置 -->   
<key>NSLocationWhenInUseUsageDescription</key>   
<string>App需要您的同意,才能在使用期间访问位置</string>   
<!-- 始终访问位置 -->   
<key>NSLocationAlwaysUsageDescription</key>   
<string>App需要您的同意,才能始终访问位置</string>   
<!-- 日历 -->   
<key>NSCalendarsUsageDescription</key>   
<string>App需要您的同意,才能访问日历</string>   
<!-- 提醒事项 -->   
<key>NSRemindersUsageDescription</key>   
<string>App需要您的同意,才能访问提醒事项</string>   
<!-- 运动与健身 -->   
<key>NSMotionUsageDescription</key> 
<string>App需要您的同意,才能访问运动与健身</string>   
<!-- 健康更新 -->   
<key>NSHealthUpdateUsageDescription</key>   
<string>App需要您的同意,才能访问健康更新 </string>   
<!-- 健康分享 -->   
<key>NSHealthShareUsageDescription</key>   
<string>App需要您的同意,才能访问健康分享</string>   
<!-- 蓝牙 -->   
<key>NSBluetoothPeripheralUsageDescription</key>   
<string>App需要您的同意,才能访问蓝牙</string>   
<!-- 媒体资料库 -->   
<key>NSAppleMusicUsageDescription</key>  
<string>App需要您的同意,才能访问媒体资料库</string> 
```

## flutter常用库
位置：./pubspec.yaml

```
# 本地存储
shared_preferences: ^0.5.3+3
# 网络请求
dio: ^2.1.13
# 全局state
scoped_model: ^1.0.1
# 数据加密 SHA-1 SHA-256 MD5 HMAC
crypto: ^2.0.6
#toast
oktoast: ^2.1.9
#状态管理
provider: ^3.0.0+1
#webview
flutter_webview_plugin: ^0.3.5
#上拉刷新&下拉加载
flutter_easyrefresh: ^1.2.7
#屏幕适配
flutter_screenutil: ^0.5.3
# A Flutter plugin for launching a URL in the mobile platform. Supports iOS and Android.
url_launcher: ^5.1.1
# #第三方登录，分享等功能
# sharesdk: ^1.1.3
#音频播放
audioplayers:
#视频播放
video_player:
# chewie: ^0.9.7
#屏幕旋转
orientation: ^1.0.5
#微信sdk
fluwx:
#图片预览
photo_view: ^0.4.2
```

### iconfont转码库:iconfont_builder

```
fonts:
  # $ iconfont_builder --from ./fonts --to ./lib/Iconfont.dart
    - family: iconfont
      fonts:
        - asset: fonts/iconfont.ttf
```
