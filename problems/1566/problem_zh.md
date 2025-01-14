## 题目背景

马老师在写高精度减法。高精度减法一开始需要比较大整数的大小关系。如果两个数都没有前导 $0$ 那很简单。但万一有前导 $0$ 似乎就麻烦一点了。为了考察一下同学们更复杂的大整数比较，于是就有了这道题。

## 题目描述

输入两个可能有前导 $0$ 的大整数，$a,b$，请输出他们谁大谁小。

- 如果 $a>b$，那么输出 `first`
- 如果 $b>a$，那么输出 `second`
- 如果 $a=b$，那么输出 `same`

## 输入格式

输入两行。

第一行为整数 $a$。

第二行为整数 $b$。

## 输出格式

输出一行，即比较的结果（`first`，`second` 或 `same`）

```input1
100
0200
```

```output1
second
```

```input2
00100
100
```

```output2
same
```

```input3

000087654321
00009876543
```

```output3
first
```


## 数据规模与约定

对于 $100\%$ 的数据，$0 \le a,b \le 10^{1000}$，$a,b$ 可能有多余的前导 $0$，保证输入的两个数算上前导 $0$ 之后的长度都不超过 $1100$。

- 子任务 1（30 分）：$0\le a,b\le 10^9$。
- 子任务 2（30 分）：两个数都没有多余的前导 $0$
- 子任务 3（40 分）：没有特殊限制。