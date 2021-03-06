# 目录

* [介绍](README.md)
* [集成Specter SDK](specterfunction/README.md)
  * [幽灵分析系统](spectersystem/README.md)
  * [引入静态库SDK](addsdklibrary/staticlib/README.md)
    * [导入静态库](addsdklibrary/staticlib/importlib.md)
    * [配置库文件](addsdklibrary/staticlib/configlib.md)
    * [配置头文件](addsdklibrary/staticlib/configheader.md)
  * [引入动态库SDK](addsdklibrary/framework/README.md)
    * [配置framework文件](addsdklibrary/framework/framework.md)
  * [代码集成功能](addcode/README.md)
    * [引入头文件](addcode/headfile/README.md)
    * [初始化Library\(常用\)](addcode/loadlibrary/README.md)
    * [上报事件\(常用\)](addcode/trackevent/README.md)
    * [计时事件\(常用\)](addcode/timeevent/README.md)
    * [清除所有计时事件](addcode/cleartimerevents/README.md)
    * [注册超级属性](addcode/registersuperprop/README.md)
    * [一次性设置超级属性](addcode/registersuperproponce/README.md)
    * [注销超级属性](addcode/unregistersuperprop/README.md)
    * [清除所有超级属性](addcode/clearsuperprop/README.md)
    * [管理用户身份](addcode/indentify/README.md)
    * [用户身份别名](addcode/createalias/README.md)
    * [存储用户配置文件](addcode/people/README.md)
      1. [设置文件属性](addcode/people/set/README.md)
      2. [递增的数字属性](addcode/people/increment/README.md)
    * [跟踪收入](addcode/trackcharge/README.md)
    * [注册推送通知](addcode/addpush/README.md)
  * [各种开关标识](switchflag/README.md)
    * [上报标识开关](switchflag/trackdata.md)
    * [摇一摇标识开关](switchflag/shake.md)
  * [SDK相关url描述](sdkurl/README.md)
  * [事件名称定义](eventname/README.md)
  * [圈选控件生成算法](selectcontrol/README.md)
  * [埋点监控描述](buriedpointmonitor/README.md)
    * [控件型](buriedpointmonitor/control/README.md)
      * 1.[普通触摸控件UIControl](buriedpointmonitor/control/uicontrol.md)
      * 2.[文本输入框控件UITextField](buriedpointmonitor/control/uitextfield.md)
      * 3.[表格控件UITableView](buriedpointmonitor/control/uitableview.md)
      * 4.[集合控件UICollectionView](buriedpointmonitor/control/uicollectionview.md)
      * 5.[网页控件UIWebView(不能圈选)](buriedpointmonitor/control/uiwebview.md)
    * [非控件型](buriedpointmonitor/uncontrol/README.md)
      * 1.[页面停留事件](buriedpointmonitor/uncontrol/pageduration.md)
      * 2.[自动埋点事件](buriedpointmonitor/uncontrol/autoevent.md)
      * 3.[首次启动App事件](buriedpointmonitor/uncontrol/firstopenapp.md)
      * 4.[App崩溃事件](buriedpointmonitor/uncontrol/exceptionevent.md)
  * [常见问题](question/README.md)
