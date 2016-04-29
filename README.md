# Homework-7
##摘要
主要研究棒球的运动，由于棒球表面具有复杂的表面结构，它在空气中旋转的时候，对飞行轨迹会产生不同的影响，同时它的转速的不同，飞行的轨迹也会不同。
参考书上的2.19的例子,以及给出的常数。  
建立一个棒球模型，阻尼系数采用课本的曲线，如果不考自身自旋的的情况下，棒球的运动与作业6中炮弹的运动情况相似，接下来，我们引入棒球的自旋，
看看此时棒球的运动轨迹会是什么样的情况。
##正文
棒球的微分方程由下式给出  
FM = S0 **w** * **v**，粗体表示矢量式  
因而可以得出棒球运动的微分方程组  
dx/dt = vx  
dvx/dt = -B2*v*vx/m  
dy/dt = -g  
dz/dt = vz  
dvz/dt = -S0*vx*w/m  
方程组的参数设定为  
S0/m = 4.1*10^(-4)  B2/m = 0.039+0.058/(1+exp((v-vd)/delta))  
给定几个初始条件来观察棒球的运动。  
[程序](https://github.com/Wangzhengwhu/Homework-7/blob/master/10.py)  
1.设定vx = 5m/s ,vy = 50m/s ,得出轨迹图如下  
![5.50](https://github.com/Wangzhengwhu/Homework-7/blob/master/5.50.png)  
2.设定vx = 10m/s ,vy = 100m/s ,得出轨迹图如下  
![10.100](https://github.com/Wangzhengwhu/Homework-7/blob/master/10.100.png)  
3.设定vx = 10m/s ,vy = 1000m/s ,得出轨迹图如下  
![10.1000](https://github.com/Wangzhengwhu/Homework-7/blob/master/10.1000.png)  
4.设定vx = 10m/s ,vy = 2500m/s ,得出轨迹图如下  
![10.2500](https://github.com/Wangzhengwhu/Homework-7/blob/master/10.2500.png)  
##结论
当vy更大时，计算机无法计算。从上面的几幅图对比，发现当vy较小时，沿着坐标轴的负方向运动，当vy>1000m/s时，沿着坐标轴的正方向运动。
数值计算出的结果在y轴方向与我的想法不太符合。
##致谢
感谢刘星辰同学提供的程序

