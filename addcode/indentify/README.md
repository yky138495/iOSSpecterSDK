# 管理用户身份

> Specter Liabrary将分配一个默认的唯一标识符（我们叫它“独特的ID”）每一个独特的用户安装你的应用。这个不同的ID被保存到设备存储，以便它将跨会话持久化。如果您选择，您可以指定自己的用户ID。如果用户在多个设备或平台上使用应用程序（例如Web和移动），这一点尤其有用。附上你自己的distinct_ids，可以使用identify:。示例如下：


```swift
    [specter identify:@"CURRENT USER DISTINCT ID"];
```

> 注意：调用 identify:一个新的ID将改变存储设备上的distinctid。用户配置文件的更新到设备的队列中，直到识别被调用