# 非控件类型的埋点监控描述

1. 普通触摸控件UIControl
 * 上报的字段名称
    * event_name：事件名称，没有圈选名称为sdk默认为ios_event_xxxxxx；圈选后名称为自定义名称
    * path：截屏数据结构中包含该值
    * event_type：ui_control
    * position_x：触摸位置的X坐标
    * position_y：触摸位置的Y坐标
    * action：动作的名称
    * 当前页面的标题路径


2. 可视化控件埋点名称
> ios_event_uicontrol(具体还要视子控件类型)
> ios_event_uitextfield
> ios_event_uitableview
> ios_event_uicollectionview
> ios_event_uiwebview