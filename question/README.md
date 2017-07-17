# 常见问题

1、可视化埋点对控件的限制
> 1. 对继承于 UITableView的控件进行可视化埋点，不可对某个 cell 进行可视化埋点。
> 1. 对继承于 UICollection的控件进行可视化埋点，不可对某个 cell 进行可视化埋点。

2、对个别特殊控件不支持可视化
> 1. UIPickerView控件
> 2. UITextView控件