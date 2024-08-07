## 题目描述

小凯手中有两种面值的金币，两种面值均为正整数且彼此互素。每种金币小凯都有无数个。在不找零的情况下，仅凭这两种金币，有些物品他是无法准确支付的。现在小凯想知道在无法准确支付的物品中，最贵的价值是多少金币？注意：输入数据保证存在小凯无法准确支付的商品。 

## 输入格式

输入数据仅一行，包含两个正整数 $a$ 和 $b$，它们之间用一个空格隔开，表示小凯手中金币的面值。

## 输出格式

输出文件仅一行，一个正整数 $N$，表示不找零的情况下，小凯用手中的金币不能准确支付的最贵的物品的价值。  

```input1
3 7
```
```output1
11
```

小凯手中有面值为 $3$ 和 $7$ 的金币无数个，在不找零的前提下无法准确支付价值为 $1,2,4,5,8,11$ 的物品，其中最贵的物品价值为 $11$。

比 $11$ 贵的物品都能买到，比如：
- $ 12 = 3 \times 4 + 7 \times 0$；
- $13 = 3 \times 2 + 7 \times1$；
- $ 14 = 3 \times 0 + 7 \times 2$；
- $ 15 = 3 \times 5 + 7 \times 0$。

## 数据范围与提示

对于 $30\%$ 的数据：$ 1 \le a,b \le 50$；  
对于 $60\%$ 的数据：$1 \le a,b \le 10^4$；  
对于 $100\%$ 的数据：$1 \le a,b \le 10^9$。