# 上报标识开关
一、上报开关是通过decide通信接口中获取，开关字段为：`report_flag`，代码如下：

``` swift
NSDictionary *config = object[@"report_config"];
if (config && [config isKindOfClass:NSDictionary.class]) {
    NSNumber *reportFlag = config[@"report_flag"];
    if (reportFlag && [reportFlag isKindOfClass:[NSNumber class]]) {
        if (reportFlag.integerValue == 1) {
            self.validationEnabled = YES;
        }else {
            self.validationEnabled = NO;
        }
    }
}
```
注意：
> 上报开关开启上报所有事件数据：
> 1. 手动埋点事件
> 2. 全埋点事件
> 3. 可视化埋点事件

> SDK默认事件包括：
> 1. 第一次打开App的上报事件
> 2. 页面停留时间事件
> 3. App崩溃事件


二、上报模式
也是通过decide通信接口中获取，开关字段为：`report_flag`，代码如下：

```swift
NSNumber *reportPattern = config[@"report_pattern"];
if (reportPattern && [reportPattern isKindOfClass:NSNumber.class]) {
    if (reportPattern.integerValue == 1) {
        self.validationMode = AutomaticEventModeVisualization;
    } else {
        self.validationMode = AutomaticEventModeAll;
    }
}                

> 分为以下两种模式：
> 1. 全埋点模式
> 2. 可视化埋点模式。



```

