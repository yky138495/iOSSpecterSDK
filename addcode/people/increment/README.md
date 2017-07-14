# 递增的数字属性

> 这是有用的，当你想保持一个运行记录的东西，如玩游戏，发送邮件，或赚取点。可以使用people increment：改变数字属性的当前值。示例如下：

```swift
    [specter.people increment:@"point count" by:@500];	
    [specter.people increment:@{
        @"dollars spent":@17,
        @"credits remaining":@-34
    }];
```

