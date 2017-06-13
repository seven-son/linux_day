# screen 软件的应用

**screen功能** 

   经常连接用ssh连接linux终端的人，在操作一些大的文件,常常不能关闭窗口，要等待，否则这个任务被杀掉，半途而废。而screen就是解决这个问题的screen的作用就是让一个或多个用户使用一个终端或多个终端多次登录同一个会话，并共享会话的所有特性。

**run 起来**

首先给你一个最简答的例子，也是我们最常用的，将一个会话挂起，重新连接(该会话并没死在后台运行)
创建   
          1 screen -S david 
          screen -S   每个screen的name
          2 screen vim a.md
挂起screen
       1 C-a d，
 
重新连接screen
         screen -r 12865

**screen基础**

在linux终端分为两种命令:
在linux终端直接查看关于screen的信息，是在linux终端显示screen的信息,还有一种是在screen软件里面使用的命令

linux终端
screen  ls  查看所有的screen连接
screen -r  id  激活screen的某个连接
screen -S yourname -> 新建一个叫yourname的session
screen -ls -> 列出当前所有的session
screen -r yourname -> 回到yourname这个session
screen -d yourname -> 远程detach某个session
screen -d -r yourname -> 结束当前session并回到yourname这个session

**screen进阶**
