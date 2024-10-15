## 题目描述

最近 33DAI 开始骑车健身了。他一看骑行记录，发现短短 $n$ 天累计骑了很长的路程。

现在给出他 $n$ 天的骑行记录，第 $i$ 天的骑行路程是 $a_i$ 千米。请问他是在第几天达到 $100$ 千米的。

## 输入格式

第一行一个整数 $n$。  

接下来一行 $n$ 个整数，即 $a_1\sim a_n$。

## 输出格式

一行一个整数，即 33DAI 是在第几天骑到 $100$ 千米的。。

```input1
9
6 10 14 25 79 34 21 41 25
```

```output1
5
```

```input2
10
20 20 20 20 10 10 20 20 20 20
```

```output2
6
```



## 数据规模与约定

对于 $100\%$ 的数据，$1\le  n \le 100$，$1\le a_i\le 100 \lt a_1+a_2+\dots + a_n$。

- 子任务 1（30 分）：保证 $n = 3$。
- 子任务 2（30 分）：保证 $a_i = 3$。
- 子任务 3（40 分）：没有特殊限制。