# 初始化Library(常用)

> 在您发送的每个事件中包含某些属性是很常见的。一般来说，这些都是关于用户的，而不是关于特定事件的，例如用户的年龄、性别或来源。
> 为了使这些功能变得更容易，您可以将这些属性注册为超级属性。如果您这样做，我们将自动将它们包括所有跟踪事件。超级属性保存到存储设备，并将始终在你的应用程序调用。Specter已经储存了一些信息作为默认的超级性能；看到一个充满Specter默认属性列表在这里。



```swift
    1. Specter *specter = [Specter sharedInstanceWithToken:@" YourSpecterToken"];
                       
    2. Specter *specter = [Specter sharedInstanceWithToken:@" YourSpecterToken" launchOptions:launchOptions];

```

