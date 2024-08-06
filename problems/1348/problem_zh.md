## 题目描述
小苞准备开着车沿着公路自驾。

公路上一共有 $n$ 个站点，编号为从 $1$ 到 $n$。其中站点 $i$ 与站点 $i + 1$ 的距离为 $v_i$ 公里。

公路上每个站点都可以加油，编号为 $i$ 的站点一升油的价格为 $a_i$ 元，且每个站点只出售整数升的油。

小苞想从站点 $1$ 开车到站点 $n$，一开始小苞在站点 $1$ 且车的油箱是空的。已知车的油箱足够大，可以装下任意多的油，且每升油可以让车前进 $d$ 公里。问小苞从站点 $1$ 开到站点 $n$，至少要花多少钱加油？

## 输入格式
输入的第一行包含两个正整数 $n$ 和 $d$，分别表示公路上站点的数量和车每升油可以前进的距离。

输入的第二行包含 $n - 1$ 个正整数 $v_1, v_2\dots v_{n-1}$，分别表示站点间的距离。

输入的第三行包含 $n$ 个正整数 $a_1, a_2 \dots a_n$，分别表示在不同站点加油的价格。

## 输出格式
输出一行，仅包含一个正整数，表示从站点 $1$ 开到站点 $n$，小苞至少要花多少钱加油。

```input1
5 4
10 10 10 10
9 8 9 6 5
```

```output1
79
```

## 提示
**【样例 1 解释】**

最优方案下：小苞在站点 $1$ 买了 $3$ 升油，在站点 $2$ 购买了 $5$ 升油，在站点 $4$ 购买了 $2$ 升油。

**【样例 2】**

见选手目录下的 road/road2.in 与 road/road2.ans。

**【数据范围】**

对于所有测试数据保证：$1 \leq n \leq 10^5$，$1 \leq d \leq 10^5$，$1 \leq v_i \leq 10^5$，$1 \leq a_i \leq 10^5$。

| 测试点 | $n \leq$ | 特殊性质 |
| :----------: | :----------: | :----------: |
| $1\sim 5$ | $8$ | 无 |
| $6\sim 10$ | $10^3$ | 无 |
| $11\sim 13$ | $10^5$ | A |
| $14\sim 16$ | $10^5$ | B |
| $17\sim 20$ | $10^5$ | 无 |

- 特殊性质 A：站点 $1$ 的油价最低。
- 特殊性质 B：对于所有 $1 \leq i < n$，$v_i$ 为 $d$ 的倍数。
