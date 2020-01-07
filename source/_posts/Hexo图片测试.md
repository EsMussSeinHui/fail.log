---
title: Hexo图片测试
tags: tryHexo
categories: Hexo
abbrlink: b16545e0
date: 2020-01-07 15:19:29
---
# hexo 图片测试
&emsp;&emsp;因为个人的习惯，自己写文档的时候，喜欢把当前文件夹下的所有文档种包含的图片，都存储在当前文件夹下的.images文件夹中。
&emsp;&emsp;但是hexo并没有提供这种方式。如下是hexo官方写的两种方式，有兴趣的可以直接查看官网 [hexo资源文件夹](https://hexo.io/zh-cn/docs/asset-folders).

<!-- more -->

## 1.放置source/images
&emsp;&emsp;这也是笔者采用的方式。将资源文件放在/source/images，在利用markdown的相对路径去获取。

## 2.插件方法
[Hexo文章中插入图片的方法](https://blog.csdn.net/Fitz1318/article/details/86548129)

但是我对这种方法有一个疑惑，即在自己写的时候是不是因为路径的问题看不到，没去测试，而且笔者更喜欢上面那种管理方式。
原因也比较简单.只要设置 vscode 插件paste images 将 图片途径改为跟目录的images就通用了。平时写作改一下习惯就可以了。
但是产生时候是 (../images/imgfilename)。虽然在vscode里面 (/images/) 和 (../images/)都可以预览。估计 (/images/) 是作为工作区的根目录下的images去寻找的(未考证)。
所以，如果是要发布的文章只要将 (../images/) 改为  (/images/) 。如果是自己的文章就不用改了，相对路径的话，适用于各种软件。之前的typora也是这样的。

官方给了一个函数 可以控制width 和 high,下次需要的时候尝试吧。

![](/images/img2020-01-07-21-00-50.png)