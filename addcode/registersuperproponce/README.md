# 一次性设置超级属性

> 如果您想存储超级属性只有一次(经常像广告或源)，你可以使用registersuperpropertiesonce：。这个函数的行为像registersuperproperties：具有相同的接口，但不能重写你已经保存的超级属性。示例如下：


> ```swift
    [specter registerSuperPropertiesOnce:@{
        @"source": @"ad-01"
    }];
```

> 这意味着，调用registersuperpropertiesonce是安全的：对每一个应用程序的负载相同的属性，它只会把它当超级属性不存在。
