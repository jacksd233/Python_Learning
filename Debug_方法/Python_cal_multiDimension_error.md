# Python计算长序列-多维数据出错

使用numpy和pandas计算 2200000*4 的数据时求和结果存在偏差。

解决方法：
（1）对每一个columns/dimension 单独计算，猜测多维运算会导致混乱？或者是多维数据量太大
（2）使用torch.tensor计算，推荐此方法，更加可靠。
