# 上报标识开关
> 上报开关是通过decide通信接口中获取，开关字段为：`report_flag`，代码如下：

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

> 全埋点事件包括：
> 1. 第一次打开App的上报事件
> 2. 页面停留时间事件
> 3. App崩溃事件



> 上报数据也具有不同的模式：全埋点模式和可视化埋点模式。



```swift
    NSDictionary *config = object[@"report_config"];
                if (config && [config isKindOfClass:NSDictionary.class]) {
                    
                    NSNumber *reportFlag = config[@"report_flag"];
                    if (reportFlag && [reportFlag isKindOfClass:[NSNumber class]]) {
                        if (reportFlag.integerValue == 1) {
                            self.validationEnabled = YES;
                        }
                        else {
                            self.validationEnabled = NO;
                        }
                    }
                    NSNumber *reportPattern = config[@"report_pattern"];
                    if (reportPattern && [reportPattern isKindOfClass:NSNumber.class]) {
                        if (reportPattern.integerValue == 1) {
                            self.validationMode = AutomaticEventModeVisualization;
                        }
                        else {
                            self.validationMode = AutomaticEventModeAll;
                        }
                    }
                }
                
```

