## regex
#### 匹配规则

---

正则表达式 | 规则 | 可以匹配
---|---|---
A | 指定字符 | A
\u548c | 指定Unicode字符 | 和
. | 任意字符 | a, b, %, 0
\d | 0~9 | 0, 1, 2, ... 9
\w | a-z, A-z, 0~9, _ | a, A, 0, _
\s | 空格, tab键 |
\D | 非数字 | S, d, +, _
\W | 非\w | $,总, ..
\S | 非\s | a, A, ...
AB* | 任意个数字符 | A, AB, ABB, ABBB
AB+ | 至少1个字符 | AB, ABB, ABBB
AB? | 0个或1个字符 | A, AB
AB{3} | 指定个数字符 | ABBB
A{1,3} | 指定范围个数字符 | AB, ABB, ABBB
AB{2,} | 至少n个字符 | ABB, ABBB
AB{0,3} | 最多n个字符 | A, ABBB

#### 复杂匹配

---


正则表达式 | 规则 | 可以匹配
---|---|---
^ | 开头 | 字符串开头
$ | 结尾 | 字符串结尾
[ABC] | [...]内的任意字符 | A, B, C
[A-F0-9xy] | 指定范围的字符 | A, ..., 9, x, y
[^A-F] | 指定范围外的字符 | X
AB\|CD | AB或CD | AB, CD
AB | CD | EFG | AB或CD或EFG | AB, CD, EFG
