### GestureDetector点击空白处无反应
behavior  HitTestBehavior 值有三个 HitTestBehavior.opaque、 HitTestBehavior.deferToChild、HitTestBehavior.translucent

`HitTestBehavior.opaque` 自己处理事件 
`HitTestBehavior.deferToChild` child处理事件
`HitTestBehavior.translucent` 自己和child都可以接收事件

### 滚动盒子
滚动到边界类型
`BouncingScrollPhysics` ：允许滚动超出边界，但之后内容会反弹回来。
`ClampingScrollPhysics` ： 防止滚动超出边界，夹住 。
`AlwaysScrollableScrollPhysics` ：始终响应用户的滚动。
`NeverScrollableScrollPhysics` ：不响应用户的滚动。

