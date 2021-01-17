# EasyTimer

给`Timer`引入中间`Target`，不再强引用原`Target`，从而不影响原`Target`的释放，不需要主动调用`timer.invalidate()`释放原`target`
!!! 原`Target`必须强引用`EasyTimer`对象，否则`Timer`会随着`EasyTimer`对象的释放而终止
