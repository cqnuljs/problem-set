## 题目描述

33DAI 拿到了一个 $n$ 行 $n$ 列的字符型的二维数组，仅由 `.#*`三种字符组成（每个元素都是三种字符之一）。这个二维数组描述了一个迷宫中的情况。`.` 为空地，`#` 为墙，`*` 为灯。

灯除了**可以照到自己的位置**，还可以往上下左右四个方向，照亮其他的空地。从灯的位置，往上下左右照亮的过程中遇到 `#` 就停止。请你计算一下图中多少位置被照亮了。

比如下面的这个地图中有两盏灯，用 `o` 描述了样例 1 的地图中灯照亮的空地。

```
..o..o
#o*ooo
..o..o
..#..o
.#ooo*
.....o
```


## 输入格式

第一行一个整数 $n$。  

接下来 $n$ 行，每行 $n$ 个字符，含义为题目所述的二维迷宫数组。

## 输出格式

一行一个整数，表示有多少个位置被照亮了。

```input1
6
......
#.*...
......
..#...
.#...*
......
```

```output1
15
```

```input2
6
......
......
......
......
......
......
```

```output2
0
```

```input3
6
*#....
#.....
...#..
..#*#.
......
...#..
```

```output3
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 30$。

- 子任务 1（30 分）：保证地图中没有墙，且仅有一盏灯
- 子任务 2（30 分）：保证地图中没有墙
- 子任务 3（40 分）：没有特殊限制
