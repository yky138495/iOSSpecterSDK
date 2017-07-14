# 计时事件(常用)

> 您可以跟踪一个动作发生的时间,比如一个图像上传或评论文章,使用timeEvent: 这将标志着“开始”你的行动,你就可以完成跟踪回调。然后时间被记录在“持续时间”属性。示例如下：



```swift

    [specter timeEvent:@"Image Upload"];
    [self uploadImageWithSuccessHandler:^{			[specter track:@"eventName"];		}];

```

