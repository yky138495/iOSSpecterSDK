# 注册推送通知

> Specer Library包括发送推送通知设备令牌Specter的支持。一旦你发送装置的标记，您可以使用Specter发送推送通知到你的应用程序。示例如下：



```swift
- (void)application:(UIApplication *)application didRegisterForRemoteNotificationsWithDeviceToken: (NSData *)deviceToken {
    Specter *specter = [Specter sharedInstance];
    [specter identify:@"13793"];
    [specter.people addPushDeviceToken:deviceToken];
 }
```

