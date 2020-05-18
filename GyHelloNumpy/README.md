> 此为Numpy学习笔记
> 代码参考https://github.com/zhmhbest/HelloNumpy。如若转载，请注明出处。
> 学习书籍：《python数据分析师修炼之道》清华大学出版社
> 《Python数据分析与大数据处理从入门到精通》北京大学出版社

- [01_创建数组]()

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