---
layout: post
title: "+_+ 编码错误？仿佛回到Python"
date: 2018-01-01 20:32:20 +0300
img: gbk.jpg
description: encodings="utf8"
categories: rwd
---
## 错误如下：
![error]({{ site.baseurl }}/assets/img/error_1.png)
 
`Error:  incompatible character encodings: GBK and UTF-8`

这啥？encoding？

一位知乎老哥的解释：
>你的项目名或者样式文件名可能带有**中文**，检查一下是否有**中文**的命名！~

于是把文件夹所有的东西找遍了都没见到一个中国字，甚至改了Ruby的配置文件，还是显示编码错误。好不容易找到一个漂亮的主题难道就这么认栽吗

---

## 解决方法
以我的情况来看，问题出在目录名是中文
```
C:\Users\博熙\Desktop\Moon-gh-pages
```
“博熙”是中文，因此只需要把本地博客移至C盘即可，便摆脱了这个问题
![error]({{ site.baseurl }}/assets/img/error_2.png)