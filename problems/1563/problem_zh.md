## 题目描述

33DAI 喜欢整数 $k$。他遇到了 $n$ 个问题。

每个问题会给你两个整数 $l,r$，请你判断 $l\sim r$ 范围内有多少个整数满足“**是 $k$ 的倍数或者个位上是 $k$**”。

## 输入格式

第一行两个整数 $n,k$。

接下来一行 $n$ 行，每行两个整数 $l,r$，即当前问题。

## 输出格式

输出 $n$ 行，每行分别是每个问题的答案。 

```input1
5 3
1 10
11 1000
111 10000
1111 100000
11111 1000000
```

```output1
3
396
3956
39555
395556

```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 1000$，$1\le k\le 9$，$1\le l\le r\le 10^9$。

- 子任务 1（30 分）：保证 $k=1$。
- 子任务 2（30 分）：保证 $r\le 1000$。
- 子任务 3（40 分）：没有特殊限制。