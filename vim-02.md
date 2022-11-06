## 基本的移动

`h j k l` ： 左 下 上 右

`g G`  : 文件开头 文件末尾

`0 ^` : 行首 非blank行首

`$ g_` : 行尾 非blank行尾

`w e` : 单词开头 单词结尾

`b ge`: 上一个单词开头 上一个单词结尾

## 操作

`x` : 剪切

`y` : 复制

`d` : 删除

`c` : 删除并进入 Insert 模式
## 组合

`[n]x` : `剪切右边n个字符

`[n]X` : `剪切左边n个字符

`yy` : 复制当前行

`y[n]w` : 复制n个字符

`y[n]l` : 复制右边n个字符

`y[n]h` : 复制左边n个字符

`y0` : 复制当前光标到行首的内容

`y$` : 复制当前光标到行尾的内容

`:m,ny` : 复制 m～n 行的内容

`yG` : 复制当前光标到文件末尾的内容

`yaw` : 复制一个单词

`yas` : 复制一个句子

`d` 组合与 y 相同




