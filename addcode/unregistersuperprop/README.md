# 初始化Library(常用)

> 首先在登陆幽灵分析平台上注册您的APP，并由此得到一个唯一的APP key，比如是 YourSpecterToken。示例如下：



```swift
    1. Specter *specter = [Specter sharedInstanceWithToken:@" YourSpecterToken"];
                       
    2. Specter *specter = [Specter sharedInstanceWithToken:@" YourSpecterToken" launchOptions:launchOptions];

```

