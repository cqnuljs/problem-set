## 题目描述

草原上有 $n$ 条蛇，编号分别为 $1,2,\cdots,n$。初始时每条蛇有一个体力值 $a_i$，我们称编号为 $x$ 的蛇实力比编号为 $y$ 的蛇强当且仅当它们当前的体力值满足 $a_x>a_y$，或者 $a_x=a_y$ 且 $x>y$。

接下来这些蛇将进行决斗，决斗将持续若干轮，每一轮实力最强的蛇拥有选择权，可以选择吃或者不吃掉实力最弱的蛇：

1. 如果选择吃，那么实力最强的蛇的体力值将减去实力最弱的蛇的体力值，实力最弱的蛇被吃掉，退出接下来的决斗。之后开始下一轮决斗。

2. 如果选择不吃，决斗立刻结束。


每条蛇希望在自己不被吃的前提下在决斗中尽可能多吃别的蛇（显然，蛇不会选择吃自己）。

现在假设每条蛇都足够聪明，请你求出决斗结束后会剩几条蛇。

本题有多组数据，对于第一组数据，每条蛇体力会全部由输入给出，之后的每一组数据，会相对于上一组的数据，修改一部分蛇的体力作为新的输入。

## 输入格式

输入文件名为 `snakes.in`。

第一行一个正整数 $T$，表示数据组数。  

接下来有 $T$ 组数据，对于第 $1$ 组数据，第一行一个正整数 $n$，第二行 $n$ 个非负整数表示 $a_i$。  
对于第 $2$ 组到第 $T$ 组数据，每组数据：  
第一行第一个非负整数 $k$ 表示体力修改的蛇的个数。  
第二行 $2k$ 个整数，每两个整数组成一个二元组 $(x,y)$，表示依次将 $a_x$ 的值改为 $y$。一个位置可能被修改多次，以最后一次修改为准。

## 输出格式

输入文件名为 `snakes.out`。

输出 $T$ 行，每行一个整数表示最终存活的蛇的条数。

```input1
2
3
11 14 14
3
1 5 2 6 3 25
```

```output1
3
1
```

```input2
2
5
13 31 33 39 42
5
1 7 2 10 3 24 4 48 5 50
```

```output2
5
3
```

## 样例 3

见附加文件中的 [snakes3.in](file://snakes3.in) 与 [snakes3.ans](file://snakes3.ans)。

## 样例 4
见附加文件中的 [snakes4.in](file://snakes4.in) 与 [snakes4.ans](file://snakes4.ans)。

## 数据范围与提示

对于 $20\%$ 的数据：$n=3$。  
对于 $40\%$ 的数据：$n\le 10$。  
对于 $55\%$ 的数据：$n\le 2\times 10^3$。  
对于 $70\%$ 的数据：$n\le 5\times 10^4$。  
对于 $100\%$ 的数据：$3\le n\le 10^6$，$1\le T\le 10$，$0\le k\le 10^5$，$0\le a_i,y\le 10^9$。保证每组数据（包括所有修改完成后的）的 $a_i$ 以不降顺序排列。