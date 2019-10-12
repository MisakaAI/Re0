# <center>Re:从<span style="color:#ee0000;">零</span>开始的<span style="color:#66ccff;">编程</span>世界</center>

<center>Re:A <span style="color:#66ccff;">program</span> world from <span style="color:#ee0000;">zero</span></center>
<center>Misaka AI</center>
<center>May 13,2019</center>
<center>lolisound@gmail.com</center>

## Introduction

记录学习过程和遇到的一些麻烦，将来遇到相似的问题可以快速找到解决方法。

## Project

- Linux
- Git
- Docker
- Python
- C
- LaTeX

## Questions & Answers

Q: 为什么是 Re?
A: 已经有一点基础，但是从零开始，重新学习。

Q: 为什么要学编程?
A: **Just for fun.**

Q: 学会编程能干什么?
A: 创造世界。
[知乎相关回答](https://www.zhihu.com/question/30257163)

Q: 我英语/数学不好，能学编程吗?
A: 肯定是学过离散数学、数据结构等知识，英语又好的程序员牛逼。
但是英语/数学不好，并不意味着不能写程序。
你看变量名可以用汉语拼音啊，看英文的文档可以用 Google Translate 啊。
我也因为不会英语，数学不好，被某个在美帝留学的程序员嘲笑过。
但是管他呢，我写程序就是兴趣使然，享受编程带给我的乐趣。
[知乎相关回答](https://www.zhihu.com/question/27947339)

Q: 关于操作系统的选择？
A: 珍爱生命，远离折腾。
> **Windows**
9102年了，请使用 *Windows 10*
\
**Linux**
入门选一个倾向于稳定的 Linux 发行版即可。(包括但不仅限于 *Ubuntu* / *Debian* / *Fedora* / *OpenSUSE* / *Manjaro*)
通常情况下，*WSL*（*适用于 Linux 的 Windows 子系统*）也是不错的选择。
不用 *RedHat* / *CentOS* 的原因是，官方源里的软件可能是上个世纪的，折腾第三方源又很麻烦，自己编译更麻烦。那么为什么不直接用官方源软件版本比较新的发行版呢？（注：与 *CentOS 8* 同时推出的 *CentOS Stream* 在一定程度上解决了该问题。）
当然，*RedHat* / *CentOS* 仍是优秀的操作系统，且很多 Linux 教程都是以 *CentOS* 为基础进行教学的。
有一定基础以后就可以根据自己的需求来选择发行版了，比如喜欢折腾的同学可以试试 *Arch Linux* 或者直接 *LFS*。
但是不要在发行版的选择中浪费太多时间，人生苦短。
但就是想体验一下不同的发行版怎么办？请妥善使用虚拟机。
\
**Mac OS**
我没用过的唯一原因就是穷，且懒得折腾黑苹果

Q: 与时俱进
A: 如果你要学一个新的技术，应当从最新的版本开始学。

选择思路应该是：
1、Stable(稳定版)
2、Latest(最新版) 

不要相信部分教程里，支持 Python 2 的库比 Python 3 要多的鬼话，那种情况只存在于 Python 3 刚问世的时候。现在还不支持 Python 3 的库大多是常年无人维护的东西了。（Python 的核心团队计划在 2020 年停止支持 Python 2。）

Q: 关于学习资料
A: 大部分情况下，能从互联网上找到各种免费的教程。 (比如 [*w3cschool*](https://www.w3school.com.cn/)、[*菜鸟教程*](https://www.runoob.com/)、[*阿里云大学*](https://edu.aliyun.com) 等)
京东当当亚马逊有活动的时候也买了很多实体书，这些我会记录在 [*Book*](./Book.md) 中
同时也请善用 *百度*、*Google* 等搜索引擎。

Q: 党争？

- Vim
- Visual Studio Code
- Tab = 4 Space
- Ubuntu / Debian

```c
/* C & C++ */
#include <stdio.h>
int main()
{
    printf("Hello, World!");
    return 0;
}
```

```css
/* css */
html {
    font-size:16px;
}
```

```python
# python3
print("Hello World!")
```
