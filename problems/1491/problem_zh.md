## 题目描述

33DAI 拿到了 $n$ 个数互不相等的数，第 $i$ 个数为 $a_i$。

如果两个位置 $i,j$，满足 $i\lt j$ 并且 $a_i > a_j$，那么我们说 $(a_i,a_j)$ 是一对逆序对。

请你找到所有逆序对中，和最大的一对，输出“和最大的逆序对”的和。（题目保证至少存在一对逆序对）。

## 输入格式

第一行一个整数 $n$。  

接下来一行 $n$ 个整数，$a_1 \sim a_n$。

## 输出格式

一行一个整数，为最大的和。

```input1
5
3 4 5 1 2 
```

```output1
7
```

## 样例解释

和最大的逆序对为 $5,2$

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 10^5$，$1\le a_i\le 10^9$。

- 子任务 1（30 分）：保证 $a_i\gt a_{i+1}$
- 子任务 2（30 分）：保证 $1\le n\le 5000$
- 子任务 3（30 分）：没有特殊限制