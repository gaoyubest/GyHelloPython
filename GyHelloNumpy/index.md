> 此为Numpy学习笔记

 [View Note](https://gaoyubest.github.io/GyHelloPython/GyHelloNumpy)

# 目录

- [01_创建数组](./01_创建数组.html)
- [02_数据调整](./02_数据调整.html)
- [03_索引_切片_迭代](03_索引_切片_迭代.html)
- [04_副本_浅拷贝_深拷贝](04_副本_浅拷贝_深拷贝.html)
- [05_基本运算](./05_基本运算.html)
- [06_统计_排序](./06_统计_排序.html)


# Numpy
- **安装numpy**
```py
pip install numpy
```
- **导入**
```py
import numpy as np
```
- Numpy的**数组对象**是齐次多维数组ndarry，一个ndarry内的数据类型相同，由正整数作为索引。数组的维度称为“**轴axe**”，轴数或维度称为数组的**秩**或**维数**

- **ndarry的属性**
```python
a = np.arange(20).reshape(4, 5)
print("创建一个4行5列的数组：")
print(a)
print("数组的轴数（维度）：", a.ndim)
print("数组的形状：", a.shape)
print("数组类型：", a.dtype.name)
print("数组元素的大小：", a.itemsize)
print("数组大小：", a.size)
print("数组a类型：", type(a))
```

- **创建数据类型**
```python
dt = np.dtype(np.int32)
print("创建整形类型:", dt)
dt = np.dtype([("2018", np.str), ("GDP", np.float)])
print("创建自定义类型:", dt)
```