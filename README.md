# TestBaiduPassword
百度网盘分享文件密码测试器

关联帖子：https://www.52pojie.cn/thread-680681-1-1.html

```
PS：如果是要使用旧版的程序请下载源码进行编译，谢谢
```

## 更新历史：

1.8.1.1（2018-11-03）

>调整内部机制，避免使用起来导致占用内存过多的问题

>修改代理功能实现，调整代理为程序内部，也就是说不影响系统的网络

>修复多线程导致 代理块 出现严重的问题

>更正一个很严重的问题：多线程导致 密码精度 缺失一个的问题

>优化大部分代理逻辑问题（具体实测）

1.8.1.0（2018-10-17）

>修复 1806 版的代理代码判断错误问题

>删除启动时判断网络代码块

>优化代理文件生成的方法（具体实测）

>优化代理的代码逻辑问题

1.8.0.6（2018-06-14）

>增加代理服务人口（测试阶段） ==》kTWO 提供技术支持

>优化逻辑代码，整理代码等

1.8.0.5（2018-05-29）

>优化判断等逻辑问题，增加安卓端APP

1.8.0.4 PRO（2018-04-13）

>增加调用API，尝试直接获取密码

1.8.0.4（2018-04-12）

>更新了线程可停止功能

>支持恢复上一次检索链接的数据

>等。。。。。

1.0.0.0（0000-00-00）

>基本的功能搭建 ==》Matrix 提供技术支持

>其它忘记了

根据 https://www.52pojie.cn/thread-629100-1-1.html 进行优化

## 功能特色：

在原本的基础上添加对链接的兼容。格式如下面：

http://pan.baidu.com/share/init?surl=xxx

https://pan.baidu.com/share/init?surl=xxx

http://pan.baidu.com/s/1xxx

https://pan.baidu.com/s/1xxx

## 一些笔记：

```
  程序的多线程坑：
  
  线程和任务是 N 对 1 ，存在重复调用问题导致方法块的冲突，以我的现在的技术是实现不了太难调
  
  线程和任务是 N 对 N ，不存在重复调用问题也就不会导致方法块的冲突，这种实现相对简单
```

## 转载声明：

本程序可以通过任何方式进行转载，但请务必保留开源的地址以便我能够及时发现 BUG 以及使用者在使用过程中出现了 BUG 也能够很好的进行反馈

## 项目贡献者：

zgcwkj 博客：http://blog.zgcwkj.cn

Matrix 博客：http://www.imwxz.com

kTWO 博客：http://www.k2zone.cn

## 本源码仅提供参考，如因本代码导致出现的任何问题和所有开发者无关
