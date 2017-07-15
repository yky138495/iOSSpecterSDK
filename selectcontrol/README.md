# 圈选控件生成算法

1. 不支持圈选的控件

> UIPickerView控件
> UITextView控件

    
2. 特殊控件(UITabBar)的处理

> SDK中圈选逻辑中，仅仅使用path作为唯一关键字；而且其他控件使用path+current_url作为唯一关键字
    