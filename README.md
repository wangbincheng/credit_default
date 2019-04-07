# credit_default
信用卡违约率分析

# 信用卡违约率分析流程

![](信用卡违约率分析流程.jpg)

# Pipeline 管道机制
使用 Pipeline 管道机制的优势，参考资料：

https://www.jianshu.com/p/9c2c8c8ef42d

https://blog.csdn.net/qq_41598851/article/details/80957893

个人理解：

Pipeline是将数据处理流程的共同部分提取出来，简化代码。

以本文最后的编程案例为例，共同部分是“数据规范化”和“使用数据分类算法”，将俩部分封装。

在每一次循环“算法”时，pipeline里头完成算法更新。GridSearchCV引用固定的pipeline，实则算法已经更新了。这样减少了多余代码的书写。
