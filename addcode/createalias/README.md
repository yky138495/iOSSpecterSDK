# 用户身份别名

> 1. 针对发送相同的distinct_id事件，个人用户触发很重要。不同distinct_ids记录的事件将被视为在Specter由不同的用户进行。
> 2. 有时可以方便地在实现中使用不同的标识符来关联用户。
> 3. 最常见的情况是注册后，当用户从一个匿名用户（匿名distinct_id）来认证用户的（认证ID）。在这种情况下，您可以为用户创建一个别名distinct_id保持一致。别名是一个字符串存储在Specter查找表，是一个匿名的distinct_id相关。一旦写好别名，是不可修改的。任何数据发送到Specter，化名为distinct_id将映射到书面使用别名的匿名distinct_id磁盘。这让你开始识别用户身份的认证不改变distinct_id最终是在Specter写的。示例如下：


```swift
    1. [specter createAlias:@"Alias" forDistinctID:specter.distinctId];
                       
    2. [specter identify:specter.distinctId];
```

