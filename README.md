# 常用简洁正则表达式 / simple-regexm in chinese
Personal learning notes about regexm, scraped and revised from https://github.com/ziishaned/learn-regex/blob/master/translations/README-cn.md. Will continue to update if necessary.

## 一、常用
### 1. 基本匹配
- “()”：匹配小括号内全部内容
- “[]”：匹配方括号内字符
- “[^]”：匹配不含方括号内字符
- “.”：匹配除换行符外的所有字符
- “\d”：匹配数字，等同于[0-9]
- “\D”：匹配非数字，等同于[^\d]
### 2. 高阶匹配
- “?”：懒惰匹配，仅匹配第一个出现的，默认贪婪匹配
- “(?=)”：正先行断言：匹配出断言前面的内容：([T|t]he)(?=fat)
- “(?!)”：负先行断言：匹配出不在断言前面的内容：([T|t]he)(?!fat)
- “(?<=)”：正后发断言：匹配出断言后面的内容：(?<=[T|t]he)(fat|mat)
- “(?<!)”：负后发断言：匹配出不在断言后面的内容：(?<![T|t]he)(fat|mat)
### 3. 逻辑语句
- “|”：或
- “\”：转义
### 4. 限定语句
- “-”：限定范围：[a-z0-9]
- “* ”：限定出现0次及以上：[a-z]*
- “+”：限定出现1次及以上：c.+t
- “?”：限定出现0/1次：[T]?he
- “{}”：限定重复出现次数
	- “[0-9]{2,3}” ：匹配2-3个数字
	- “[0-9]{2,}”：匹配2个以上数字
	- “[0-9]{2}”：匹配2个数字
## 二、补充
- “^”：匹配开头
- “$”：匹配结尾
- “\w”：匹配所有字母数字，等同于[a-zA-Z0-9_]
- “\W”：匹配所有非字母数字，等同于[^\w]
- “\s”：匹配所有空格字符，等同于[\t\n\f\r\p{Z}]
- “\S”：匹配所有非空格字符，等同于[^\s]
- “\f”：匹配一个换页符
- “\n”：匹配一个换行符
- “\r”：匹配一个回车符
- “\t”：匹配一个制表符
- “\v”：匹配一个垂直制表符

整理自：[learn-regex_GitHub ](https://github.com/ziishaned/learn-regex/blob/master/translations/README-cn.md)
对原博客内容作了适度修改，更贴合中文正则使用。
