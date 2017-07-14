# 跟踪收入

> 1. Specter便于分析你从个人客户赚取的收入。通过将收费与用户配置文件相关联，您可以比较不同客户段的收入，并计算诸如终身价值之类的东西。
> 2. 你可以跟踪people的单个交易trackcharge:。这个调用将增加交易的个人用户配置文件，这也将反映在Specter收入报告。示例如下：

```swift
    [specter.people trackCharge:@(100.77)];
    [specter.people trackCharge::@25 withProperties:@{
        @"$time":@"2016-01-02T00:00:00"
    }];
```

