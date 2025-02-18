## 题目描述

33DAI 最近在玩 《黑神话：悟空》。他拿到了一个道具 “争先红葫芦”。

33DAI 操纵的游戏角色“悟空”有一个属性是**气血值**，气血值有一个上限 $x$，“悟空”的初始气血值为 $x$。气血值小于等于 $0$ 时“悟空”就被打败了。

“悟空”可以使用**争先红葫芦**来恢复游戏角色的气血值，最多使用 $n$ 次。
- 第一次可以把气血值变为 $x$。
- 后面每次可以把气血值增加 $\lfloor \frac{x}{3}\rfloor$（即 $x$ 的 $\frac{1}{3}$ 下取整）。如果增加完会大于 $x$，则只会变为 $x$。

33DAI 正在操纵“悟空”与“广智”战斗，“广智”一共进行了 $m$ 次攻击，第 $i$ 次攻击会把“悟空”的气血值减少 $a_i$。每次被攻击后“悟空”都可以使用若干次争先红葫芦（或者不使用）。

请问 33DAI 利用争先红葫芦会不会被打败。如果会被打败，请输出是在第几次攻击时被打败的。如果不会被打败，请输出 $-1$。

## 输入格式

第一行为三个数 $x,n,m$。

第二行为 $m$ 个数 $a_1\sim a_m$。


## 输出格式

如果会被打败，请输出是在第几次攻击时被打败的。如果不会被打败，请输出 $-1$。

```input1
100 4 5
50 45 60 60 70
```

```output1
-1
```

一种使用葫芦的方案为：

- 初始气血值为 $100$
- 第一次攻击后气血值为 $50$
- 第二次攻击后气血值为 $5$，此时使用 $1$ 次葫芦，气血值恢复为 $100$
- 第三次攻击后气血值为 $40$，此时使用 $2$ 次葫芦，每次恢复 $33$ 气血，气血值恢复为 $100$。
- 第四次攻击后气血值为 $40$，此时使用 $1$ 次葫芦，恢复 $33$ 气血，气血值恢复为 $73$。
- 第五次攻击后气血值为 $3$

```input2
100 100 1
101
```

```output2
1
```

一次攻击后，悟空就被打败了。

```input3
100 0 5
1 1 98 1 1
```

```output3
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le x \le 100$，$0\le n,m\le 100$，$0\le a_i\le 10^9$。

- 子任务 1（30 分）：保证“悟空”不会被打败。
- 子任务 2（30 分）：保证 $x=1$。
- 子任务 3（40 分）：没有特殊限制。