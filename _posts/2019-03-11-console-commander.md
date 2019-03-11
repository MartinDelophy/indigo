---
title: "console-commander"
layout: post
date: 2019-02-17 12:48
tag: javascript;node
category: blog
author: martindelophy

---

**javascript 命令行自定义指令**
今天看了导师搭了一个脚手架，看到里面有一个自定义指令研究了一下

1.在package.json中加入
```
  "bin": {
    "测试指令": "***.js"
  }
```
2.在跳转的 ***.js 中加入
```
#!/usr/bin/env node
...... some code start here
```
