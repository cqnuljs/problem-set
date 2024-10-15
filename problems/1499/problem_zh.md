## 题目描述

如题，你需要维护这样的一个数对（即两个数），支持如下几种操作


1. 在某个历史版本上修改某一个位置上的值
2. 访问某个历史版本上的某一位置的值

此外，每进行一次操作（**对于操作2，即为生成一个完全一样的版本，不作任何改动**），就会生成一个新的版本。版本编号即为当前操作的编号（从1开始编号，版本0表示数对的初始状态）

## 输入格式

输入的第一行包含一个正整数 $M$， 表示操作的个数。

第二行包含两个整数，即数对的初始状态，依次为第一个数 $x$ 和第二个数 $y$。

接下来 $M$ 行，第 $i$ 行包含 4 或 3 个整数，代表两种操作之一：

1. 对于操作1，格式为 $v_i \ 1 \ {loc}_i \ {value}_i $，即在版本 $v_i$的基础上，复制一份生成一个新的版本，并将第 ${loc}_i$ 个数（${loc}_i$ 为 $1$ 或 $2$），修改为 $ {value}_i $。
2. 对于操作2，格式为 $v_i \ 2 \ {loc}_i$，即在版本 $v_i$的基础上，复制一份生成一个新的版本，并输出第 ${loc}_i$ 个数（${loc}_i$ 为 $1$ 或 $2$）。

## 输出格式

输出包含若干行，依次为每个操作2的结果。

```input1
6
30 40
0 1 2 50
0 1 1 60
1 2 1
1 2 2
2 2 2
5 2 1 
```

```output1
30
50
40
60
```

## 样例解释

- 版本 $0$：初始版本，数对为 `30, 40`
- 版本 $1$：`0 1 2 50`，基于版本 $0$ 复制一份，并把第二个数改为 50，得到的数对为 `30, 50`
- 版本 $2$：`0 1 1 60`，基于版本 $0$ 复制一份，并把第一个数改为 60，得到的数对为 `60, 40`
- 版本 $3$：`1 2 1`，基于版本 $1$ 复制一份，得到的数对为 `30, 50`，并输出第一个数 `30`
- 版本 $4$：`1 2 2`，基于版本 $1$ 复制一份，得到的数对为 `30, 50`，并输出第二个数 `50`
- 版本 $5$：`2 2 2`，基于版本 $2$ 复制一份，得到的数对为 `60, 40`，并输出第二个数 `40`
- 版本 $6$：`5 2 1`，基于版本 $5$ 复制一份，得到的数对为 `60, 40`，并输出第一个数 `60`

## 数据范围

对于 $100\%$ 的数据，保证：
- $1\le M\le 100$
- $v_i\lt i$
- ${loc}_i$ 为 $1$ 或 $2$
- $1\le x,y,{value}_i\le 100$ 

子任务划分：
- 子任务 1（30 分）：只有操作 2
- 子任务 2（30 分）：保证 ${loc}_i=1$
- 子任务 3（40 分）：没有特殊限制