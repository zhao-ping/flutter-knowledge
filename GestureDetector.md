### GestureDetector点击空白处无反应
behavior  HitTestBehavior 值有三个 HitTestBehavior.opaque、 HitTestBehavior.deferToChild、HitTestBehavior.translucent

`HitTestBehavior.opaque` 自己处理事件 
`HitTestBehavior.deferToChild` child处理事件
`HitTestBehavior.translucent` 自己和child都可以接收事件

### 无边界约束盒
最大宽度`double.INFINITY`

### 从下方出现的弹框
`showModalBottomSheet`
