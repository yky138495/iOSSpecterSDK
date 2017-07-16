# 控件类型的埋点监控描述二

2. 文本输入框控件UITextField
 * 上报的字段名称
    * event_name：事件名称，没有圈选名称为sdk默认为ios_event_uitextfield；圈选后名称为自定义名称。
    * path：截屏数据结构中包含该值
    * event_type：ui_textfield
    * position_x：触摸位置的X坐标
    * position_y：触摸位置的Y坐标
    * action：动作的名称
    * 当前页面的标题路径
    *** 
    
 * 圈选控件字段
    * current_url：当前页面的标题路径
    * event_name：事件名称
    * control_event：控件的事件值，为64
    * path: 圈选控件的path值，生成path的条件如下：
       > 1. IsViewVisible：判断控件在当前界面是否可见
       2. UserInteractionEnabled：判断控件是否开启交互功能
       3. 对于控件类型为UIPickerView不生成path，即不能圈选
       
       只有i和ii两个条件均成功，才能圈选，即生成path。
    * event_type：ui_control
    ***
    

 