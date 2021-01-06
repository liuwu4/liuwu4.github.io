---
title: 正则表达式
date: 2020-12-28 14:09:37
category: Pattern
---

### [非获取匹配(预查匹配)`?:` `?=` `?!` `?<!` `?<=`](https://www.runoob.com/regexp/regexp-metachar.html)

| 序号 |  类型   |      语法       |                                               说明                                                |
| :--: | :-----: | :-------------: | :-----------------------------------------------------------------------------------------------: |
|  1   | **?:**  | rule1(?:rule2)  | **查找满足`()`中的值,在向左查找满足 `rule1` 规则的值** 结果不包含满足 `rule2` 的值 _查找`()`左边_ |
|  2   | **?=**  | rule1(?=rule2)  |  **查找满足`()`中的值,在向左查找满足 `rule1` 规则的值** 结果包含满足 `rule2` 的值 _查找`()`左边_  |
|  3   | **?!**  | rule1(?!rule2)  |         **当前值满足 `rule1` 下一次值不能满足 `rule2`** 结果不包含失败的值 _查找`()`左边_         |
|  4   | **?<=** | (?<=rule2)rule1 |      **查找满足`rule2`开头的值且后续值满足 `rule1`** 结果开头不能满足`rule2` _查找`()`右边_       |
|  5   | **?<!** | (?<!rule2)rule1 |                   **满足整个规则** 结果开头不能满足`rule2rule1` _查找`()`右边_                    |