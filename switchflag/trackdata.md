# 上报标识开关
> 上报开关是通过decide通信接口中获取，开关字段为：`report_flag`，代码如下：


``` swift
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

```


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

