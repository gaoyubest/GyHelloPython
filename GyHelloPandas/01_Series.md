# 序列
- 包含两个对象：**索引和数据**。
- **Series**()常用参数：
   - **data**：创建序列对象的原始数据，可以是列表、字典
   - **index**：索引/标签，类似于数组下标
   - **dtype**：数据类型
   - **copy**：是否创建数据副本 

#### 1、创建空序列
```py
data = pd.Series()
print("默认的空序列：", data)   # Series([], dtype: float64)
```

#### 2、通过数值创建序列
```py
data = pd.Series(5, index=[0, 1, 2])
# 0    5
# 1    5
# 2    5
data = pd.Series(5, index=["a", "b", "d"])
```

#### 3、通过Numpy数组创建序列
```py
data = np.array(['hello', 'world', 'python'])
data = pd.Series(data)
# 0     hello
# 1     world
# 2     python
```

#### 4、通过字典创建序列
```py
data = {
    "name": "Ivy",
    "age": 10
}
data = pd.Series(data)
```

#### 5、通过列表创建序列
```py
series = {
          "name": pd.Series(["Wilson", "Bruce", "Chelsea"]),
          "age": pd.Series([15, 24, 19]),
          "gender": pd.Series(["man", "man", "woman"])
}
df = pd.DataFrame(series)
```


