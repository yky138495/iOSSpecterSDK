# 设置文件属性

> 1. 设置用户 13793的 “Plan”属性的值为 “Premium”。示例如下：
```swift
    [specter.people set:@"Plan" to:@"Premium"];
```
> 2. 在用户13793的配置文件里，将设置一个“Plan”属性，带有一个值“Premium”。在Specter中如果没有一个配置文件存在distinct_id 13793的，一个新的配置文件将被创建。如果用户13793在其配置文件中已经有一个名为“Plan”的属性，则旧值将用“高级”覆盖。
