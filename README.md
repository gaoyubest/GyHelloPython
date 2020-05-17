# Numpy
- **安装numpy**
```py
pip install numpy
```
- **导入**
```py
import numpy as np
```
- Numpy的**数组对象**是ndarry，一个ndarry内的数据类型相同，由正整数作为索引。数组的维度称为“**轴**”

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