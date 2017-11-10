# midterm homework——pygame（打砖块）
王子睿 2015301020068
---

## 功能划分
现将一个打砖块的主要功能分解如下：
1）实现一个小球在屏幕上移动
2）碰到边缘要能够反弹
3）挡板绘制和移动
4）砖块的绘制
5）游戏流程和控制逻辑
6）绘制文字显示游戏信息
7）加个背景音乐
这几个功能应该都是在一定时间内能够实现的简单功能，而只要将他们合理的组合起来就是一个完整的打砖块游戏了~

## 小球的绘制和移动
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/1.png)
下面画个会动的小球吧：
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/2.png)
## 碰撞检测
小球一出来就开始跑，一会儿就不见了。这一步要让它碰到边界就反弹回去。
## 挡板绘制和移动
然后就是实现一个能够根据玩家输入移动的挡板，来阻挡小球。
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/3.png)
## 砖块的绘制
首先要有个数组记录砖块是否已经被打掉了，然后把未被打掉的绘制在窗口上部
初始化砖块二维数组
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/4.png)
## 游戏流程和控制逻辑
1）把砖块打破
2）被挡板挡住才返回，落没挡住则要减少一条生命
3）生命用完了则Game Over
4）砖块打完了要进入下一关或宣告胜利
## 绘制文字显示游戏信息
合理计算分数，并设置过关：
比如每过一关加1000分，打完所有砖块则进入下一关。
左下角显示游戏信息，如关卡、分数、生命等，游戏结束显示Game Over信息
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/5.png)
![](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/6.png)
## 完整代码
[代码](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/source%20code)
## 试玩
[试玩的视频](https://github.com/wzrwisdom/compuational_physics_N2015301020068/blob/master/midterm%20homework/Video_20171110111231.wmv)
