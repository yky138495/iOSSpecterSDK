# 圈选控件生成算法

1. 不支持圈选的控件
> UIPickerView控件
> UITextView控件

2. 特殊控件(UITabBar)的处理
> SDK中圈选逻辑中，仅仅使用path作为唯一关键字；而且其他控件使用path+current_url作为唯一关键字

3. 对应同一界面上有多个类型相同的控件，出现一下情况的处理
    > 1. 当动态出现控件时，一般设置specterViewId或者tag，当然具有title的控件也可以使用title;
    > 2. 如果specterViewId、tag、控件的标题都不存在时，这个时候就要获取控件对象所在的索引值，但是获取索引时，系统给的subviews数组不是按照控件对象的位置排序的，这时，就要根据同类型控件对象的x和y进行升序排序;
    > 3. current_url 目前版本中使用当前界面的类名代替.