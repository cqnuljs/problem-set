## 题目描述

给定一个长度为 $5$ 的仅由小写英文字母构成的字符串 $s$，请判断它是否是由 $5$ 个连续的字符组成的。

## 输入格式

输入一个字符串 $s$。

## 输出格式

如果是连续的字符组成的，输出 `Yes`；否则输出 `No`。

```input1
abcde
```

```output1
Yes
```

```input2
iljkh
```

```output2
Yes
```

## 样例解释

是由连续的五个字符 `hijkl`。

```input3
dcxbe
```

```output3
No
```

## 数据规模与约定

对于 $100\%$ 的数据，保证所有字符互不相同。

- 子任务 1（30 分）：保证五个字符按照字典序从小到大排列。
- 子任务 2（30 分）：保证每个字符都是 `abcde` 中的某一个。
- 子任务 3（40 分）：没有特殊限制。