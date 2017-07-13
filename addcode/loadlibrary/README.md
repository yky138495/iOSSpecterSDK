# 初始化Library(常用)

> 首先在登陆幽灵分析平台上注册您的APP，并由此得到一个唯一的APP key，比如是 YourSpecterToken。示例如下：



```swift
    Specter *specter = [Specter sharedInstanceWithToken:@" YourSpecterToken"];                       Specter *specter = [Specter sharedInstanceWithToken:@" YourSpecterToken" launchOptions:launchOptions];

```

