# 注册超级属性

> 1. 在您发送的每个事件中包含某些属性是很常见的。一般来说，这些都是关于用户的，而不是关于特定事件的，例如用户的年龄、性别或来源。

> 2. 为了使这些功能变得更容易，您可以将这些属性注册为超级属性。如果您这样做，我们将自动将它们包括所有跟踪事件。超级属性保存到存储设备，并将始终在你的应用程序调用。Specter已经储存了一些信息作为默认的超级性能；看到一个充满Specter默认属性列表在这里。

> 3. 设置超级性能，叫registersuperproperties:

> 4. 发送一个“name：niwodai”的属性，将被发送给所有的track 回调。示例如下:
```swift
    [specter registerSuperProperties:@{@"name": @"niwodai"}];
```
> 5. 向前一步：每当您发送一个事件时，超级属性将包含为属性，示例如下:
```swift
    [specter track:@"eventName" properties: @{
        @"prop1": @"value1"
    }];
```
> 6. 后退一步：调用上报事件，就像直接添加的属性，示例如下:
```swift
    [specter track:@"eventName" properties: @{
        @"prop1": @"value1",
        @"name": @"niwodai"
    }];
```
