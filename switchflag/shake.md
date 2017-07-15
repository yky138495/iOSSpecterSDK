# 摇一摇标识开关
> 该功能是在UIViewController的分类中增加的，文件：`UIViewController+ShakeAndCutter.m`,开关标识开关代码如下：

```swift
- (void) motionEnded:(UIEventSubtype)motion withEvent:(UIEvent *)event {
    //摇动结束
    if (event.subtype == UIEventSubtypeMotionShake) {// 判断是否是摇动结束
        NSLog(@"摇动结束");
        if ([Specter sharedInstance].enableShake) {
            [[Specter sharedInstance] connectToABTestDesigner];
        }
    }
}
```

