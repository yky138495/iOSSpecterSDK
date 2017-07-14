# 上报事件(常用)

> 幽灵SDK支持手动事件上报，并且可携带自定义的属性，示例如下：

```swift
    1. [specter track:@"eventName"];
                       
    2. [specter track:@"eventName" properties: @{@"prop1": @"value1", @"prop2": @"value2"}];

```

