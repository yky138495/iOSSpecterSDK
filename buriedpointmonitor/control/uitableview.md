# 控件类型的埋点监控描述三

3.表格控件UITableView
 * 上报的字段名称
    * event_name：事件名称，没有圈选名称为sdk默认为ios_event_uitableview；圈选后名称为自定义名称
    * path：截屏数据结构中包含该值
    * event_type：ui_tableview
    * table_delegate：表格控件的代理类
    * cell_section：表格控件的区块索引
    * cell_index：表格控件的行索引
    * current_url：当前页面的标题路径
    *** 
    
 * 圈选控件字段
    * current_url：当前页面的标题路径
    * event_name：事件名称
    * path: 圈选控件的path值，生成path的条件如下：
       > 1. IsViewVisible：判断控件在当前界面是否可见
       2. UserInteractionEnabled：判断控件是否开启交互功能
       
       只有i和ii两个条件均成功，才能圈选，即生成path。
    * table_delegate：表格控件的代理类
    * event_type：ui_tableview
    ***
    
 * 注意：对于UITableView控件只能圈选整个表格控件，不能圈选里面的UITableViewCell子控件。

 