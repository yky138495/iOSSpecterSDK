# 控件类型的埋点监控描述五

5. 网页控件UIWebView(不能圈选)
 * 上报的字段名称
    * event_name：事件名称，sdk默认为ios_event_uiwebview
    * event_type：ui_webview
    * webview_loadstate：有三种状态值：start/finished/failure
    * webview_url：链接的url地址
    * webview_error：网页打开失败的原因
    * 当前页面的标题路径
    ***
    
 