#my little program  

1、原生js实现打地鼠游戏  

http://hunterfront.github.io/little-program/beatmole  

参考原型图：  

![](https://github.com/HunterFront/little-program/blob/master/images/game1.png)  

相关技术：HTML、CSS、JS  

项目需求：实现一个web页面的打地鼠游戏  

功能需求：  

	随机在界面中生成地鼠  

	击中地鼠的同时实现一定的交互效果（地鼠、锤子状态有变化）  

	记录分数、关卡，并计算命中率  

	实现游戏的开始、暂停和重新开始功能  

	游戏结束时，显示成绩  

页面事件：  

1.	点击开始按钮游戏开始，启动定时器  

2.	点击暂停游戏暂停，清除定时器  

3.	点击重新开始，刷新页面  

4.	点击提示框的确定键，隐藏modal框，回到游戏界面  

5.	点击游戏界面的格子，改变锤子的状态，记录点击次数，若击中分数＋1，计算命中率  

数据结构：{x:x,y:y,src:’…’};  

实现流程：  

1、	显示界面：游戏界面由一个table及里面的td构成，生成一个4*4的网格，网格的大小85px；  

2、	点击开始按钮，游戏开始，随机生成地鼠；	  

详细分析：每次产生的地鼠的数量随机[1,2,3]个，根据关卡难度分配个数产生的概率，关卡越难产生数量多的概率越大，产生的每个地鼠为其随机分配停留的时间，关卡越难分配的总时间越短，即每个地鼠分配的单个时间也会变短（每个地鼠分配的时间也按一定比率进行分配，达到参差不齐的效果）  

3、鼠标点击地鼠，点到则立即让地鼠进洞，分数加1，记录总点击次数并计算命中率；没有点到，记录总点击次数，计算命中率。  




2、原生js实现贪吃蛇游戏  

http://hunterfront.github.io/little-program/snake
