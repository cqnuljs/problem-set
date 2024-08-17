## 问题陈述

有 $N$ 个盘子，编号为 $1, 2, \ldots, N$ 。最初对于每个 $i$ ( $1 \leq i \leq N$ )，第 $i$ 个盘子上有 $a_i$ ( $1 \leq a_i \leq 3$ )块寿司。

太郎会重复执行以下操作，直到所有寿司都被吃掉：

- 掷一个骰子，骰子上显示的数字 $1, 2, \ldots, N$ 的概率相等，结果为 $i$ 。如果盘子 $i$ 上有寿司，就吃掉其中一个；如果没有，就什么都不吃。

求在所有寿司都被吃掉之前执行操作的期望次数。

## 限制因素

- 所有输入值均为整数。
- $1 \leq N \leq 300$
- $1 \leq a_i \leq 3$ 

## 输入

输入内容由标准输入法提供，格式如下：

- $N$
- $a_1$ $a_2$ $\ldots$ $a_N$

## 输出

打印在所有寿司被吃完之前执行操作的预期次数。如果相对差值不大于 $10^{-9}$ ，则认为输出正确。

```input1
3
1 1 1
``` 

```output1
5.5
```

吃掉第一块寿司前的预期操作次数为 $1$ 。之后，吃第二个寿司前的预期操作次数为 $1.5$ 。之后，吃第三个寿司前的预期操作次数为 $3$ 。因此，预计操作总数为 $1 + 1.5 + 3 = 5.5$ 。

```input2
1
3
``` 

```output2
3
```

也接受诸如 `3.00`、`3.000000003` 和 `2.999999997` 等输出。

```input3
2
1 2
``` 

```output3
4.5
``` 

```input4
10
1 3 2 3 3 2 3 2 1 3
``` 

```output4
54.48064457488221
``` 

## 来源

https://atcoder.jp/contests/dp/tasks/dp_j