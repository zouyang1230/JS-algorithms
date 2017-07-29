# JS-数据结构与算法

### 笔记记录：

1、寻路搜索模式(3种)
- 深度优先搜索:
    - 深度优先搜索过程简要来说是对每一个可能的分支路径深入到不能再深入为止，而且每个节点只能访问一次.
    - 也就是从起点找到相邻的，再从相邻的，找到下一个相邻的，一层层往下查找，一直搜索到目标点。它并没有办法找到最优的路线，可能会绕一大圈才找到目标点。


- 广度优先搜索，又叫宽度优先搜索（需考虑性能）：
    - 宽度优先搜索算法（又称广度优先搜索）是最简便的图的搜索算法之一，这一算法也是很多重要的图的算法的原型。属于一种盲目搜寻法，目的是系统地展开并检查图中的所有节点，以找寻结果。换句话说，它并不考虑结果的可能位置，彻底地搜索整张图，直到找到结果为止。
    - 通俗来讲，它的搜索像网状的，从一点像四周扩散，再从下一个点的四周继续扩散，如同病毒式分裂一样，扩散搜索。因为它搜索的范围很大，每条线路都要去搜索，很难保证性能。


- 启发式搜索（最优路线）:

    - 启发式搜索 又称为有信息搜索(Informed Search)，它是利用问题拥有的启发信息来引导搜索，达到减少搜索范围、降低问题复杂度的目的，这种利用启发信息的搜索过程称为启发式搜索。所以它又能保证性能，又能找到最优路线的搜索。有点像人类的思维。
    - 代表性的是[A*寻路算法](http://www.zouyang1230.com/project/jssf/axl.html)：<br />
    ![A*寻路](https://github.com/zouyang1230/JS-algorithms/raw/master/images/axl.gif)
    - 算法原理：如下图
    ![A*寻路算法原理图](https://github.com/zouyang1230/JS-algorithms/raw/master/images/axl2.jpg)<br />
    - 使用公式（A*估价函数）：
        - f(n)  =  g(n) + h(n)，f(n)是从下图A起始点到目标点B的距离，g(n)和h(n)如下图所示路径距离，g(n)与h(n)的和就是f(n)距离。2条路径的f(n)值相比，就能得到哪条路径更短。
        - ![A*寻路算法图示](https://github.com/zouyang1230/JS-algorithms/raw/master/images/axl2.gif)
        - f(n)是n节点的估价函数
        - g(n)是初始点到n节点的实际代价（实际代价：一个点到另一个点的最短路径）
        - h(n)是n节点到目标点的实际代价

2、行列互换算法
- 互换前：
![未互换前](https://github.com/zouyang1230/JS-algorithms/raw/master/images/hlhh1.jpg)
- 互换后：
![未互换前](https://github.com/zouyang1230/JS-algorithms/raw/master/images/hlhh2.jpg)
- 分别采用递归与取模2种方式实现：[测试链接](http://www.zouyang1230.com/project/jssf/hlhh.html) 
- 行列互换算法可以用于连连看等消除游戏

<br />
3、未完待续








