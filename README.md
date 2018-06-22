# How-to-do-nodeppt
# 根据nodeppt官方学习指导
> 1.安装：npm install -g nodeppt
> 2.查看版本：nodeppt -v
> 3.启动：nodeppt start -p <未使用的端口>
> 4.配置：
```html
title: nodeppt markdown 演示
speaker: Theo Wang
url: https://github.com/ksky521/nodePPT
transition: slide
files: /js/demo.js,/css/demo.css

/*
title: 这是演讲的题目
speaker: 演讲者名字
url: 可以设置链接
transition: 转场效果，例如：zoomin/cards/slide
files: 引入js和css的地址，如果有的话~自动放在页面底部
*/
```

> 5.关闭:
关闭nodeppt服务的时候，我用ctrl+z实现了关闭，发现我之前开启的端口号都不能使用了，原因我虽然把服务关了，但是并没有关闭进程，这样的话，之前开启的端口都不能使用了。解决办法：可以使用ps -ef | grep username 可以查看这个username开启的进程有哪些，也可以使用netsta -nap | grep node查看node相关的端口状态，然后使用kill -9 <进程ID>杀死进程即可。

当然最简单的办法就是：使用ctrl+c关闭nodeppt服务，这样的话进程同时会被干掉。
##6.例子：http://js8.in/nodeppt/
