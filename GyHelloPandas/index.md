# Pandas

> 此为Pandas学习笔记

 [View Note]()

# 目录

- [01_Series](./01_Series.html)
- [02_DataFrame](./02_DataFrame.html)
- [03_访问数据](03_访问数据.html)
- [04_基础功能](04_基础功能.html)
- [05_统计分析](./05_统计分析.html)
- [06_时间数据](./06_时间数据.html)
- [07_数据清洗](./07_数据清洗.html)
- [08_多维度分析_透视表_交叉表](./08_多维度分析_透视表_交叉表.html)
- [09_读写MySQL数据库](./)


# 导入
```py
import pandas as pd
```

# 数据结构
- Pandas主要基于**两个核心数据结构**：
- **序列（Series）**：包含同种数据类型的`一维数组`，可以是整数型、浮点型，大小固定。
- **数据帧（DataFrame）**：`二维数组`，可理解为表格，包含多个列，每一列数据类型相同，列之间可以不同，大小可变。