## 题目描述

输入一个十进制小数 $n$。

请按照保留 $9$ 位小数的形式（多余的数位直接略去），输出它对应的二进制数。

## 输入格式

一个数 $n$。

## 输出格式

$n$ 对应的二进制数。

```input1
0.75
```

```output1
0.110000000
```


```input2
0.11
```

```output2
0.000111000
```


```input3
0.3
```

```output3
0.010011001
```

## 数据规模与约定

对于 $100\%$ 的数据，保证 $0\lt n\lt 1$，且小数部分最少有一位，最多只有 $9$ 位。

- 子任务 1（60 分）：保证 $n$ 的小数部分只有一位。
- 子任务 2（40 分）：没有特殊限制。

Round 30 我稍微仁慈一点了，大家可以考虑一下如果输入的位数和输出的位数能到 $10^3$ 时该怎么做。