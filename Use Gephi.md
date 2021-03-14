# Use Gephi

### 一.获取数据的方式

##### 1.手动在画布上绘制

【略】

##### 2.在数据资料界面中手动输入

【略】

##### 3.CSV文件导入数据

【文件】->【输入电子表格】 可以导入节点也可以导入边的数据，一般都是导入边的数据。

##### 4.随机生成数据

【略】

##### 5.其他格式文件

gexf

##### 6.从服务器或者本地导入数据库读取数据

【输入数据】->【边名单】

##### 7.在Internet中应用代理服务器

【下载http代理插件】

##### 8.通过邮件读取数据

### 二.概览界面和五大工作栏

#### 1.图界面

![](F:\vacation\gephi\img\canvas.png)

进行的都是一些简单的基本操作，但是不适合处理大规模的数据。

(1).节点的移动

(2).节点的放大缩小

(3).节点的颜色调整

(4).边粗细的调整

(5).标签的编辑

(6).节点的编辑

#### 2.Function

从Ranking->Layout->Statistics->Partation->Filter

##### (1).Partation

###### 1.功能

把节点中，值相同的节点归为一类，并以不同的颜色大小或者标签的颜色大小进行区分。分割的依据可以来源为统计的结果，也可以是节点自己本身带有的值。

###### 2.使用栏

![Partation](F:\vacation\gephi\img\Partation.png)

###### 3.使用逻辑

【操作比较简单，参数可见Statistic和Ranking】

###### 4.呈现

![Partation2](F:\vacation\gephi\img\Partation2.png)



##### (2).Ranking

###### 1.功能

根据一些值对节点和标签进行归类排序，并把排序的结果用大小，颜色等形式应用到节点，标签上。

###### 2.使用栏

![](F:\vacation\gephi\img\Rank.png)

###### 3.使用逻辑

![](F:\vacation\gephi\img\Rank2.png)

###### 4.呈现

![](F:\vacation\gephi\img\Rank3.png)

应用了所有的Rank方法  :）

##### (3).Layout

###### 1.功能

对节点进行聚类，能够直观的表现出节点之间的关系。

###### 2.使用栏

![](F:\vacation\gephi\img\Layout.png)

###### 3.使用逻辑

![](F:\vacation\gephi\img\Layout2.png)

###### 4.呈现

![](F:\vacation\gephi\img\Layout3.png)

![Layout4](F:\vacation\gephi\img\Layout4.png)

（我好像也没有看出来啥规律:)   ）

###### *额外（布局的描述）：

1.力引导布局的描述

根据边的权重以及节点的数值，按照胡克定律以及库仑定律将力作用在节点和边上，能够完成很好的聚类，显示出节点间的亲疏关系。

2.胡一凡布局的描述

【今后补充】

*一些对布局的描述：

https://www.omegaxyz.com/2020/02/01/graph-layout/

##### (4).Statistics

###### 1.功能

根据节点和边的数值，对不同的量进行计算并保存结果，可以作为排列和分割操作的依据，相当于为节点和边增添了新的属性。

###### 2.使用栏

![](F:\vacation\gephi\img\Statistics.png)

###### 3.使用逻辑

![Statistics2](F:\vacation\gephi\img\Statistics2.png)

###### 4.呈现

![Statistics3](F:\vacation\gephi\img\Statistics3.png)

​                                                                                                      【模块化后的图像】

###### *一些统计的概念和算法

1.度：节点所连接边的数量，与之相关的有入度，出度（有向图），加权度等。

2.PageRank算法：

https://baike.baidu.com/item/google%20pagerank/2465380?fromtitle=pagerank&fromid=111004&fr=aladdin

3.连接部件，DFS算法：

https://www.cnblogs.com/mfrbuaa/p/3814912.html

4.一种模块化算法，Louvain算法：

https://blog.csdn.net/xuanyuansen/article/details/68941507

5.特征向量中心性的说明：

https://www.cnblogs.com/miaobo/p/12485574.html

6.计算点击次数，HITS算法：

https://blog.csdn.net/duguiminer/article/details/46325665

##### (5).Filter

###### 1.功能

设置条件根据节点的属性对节点进行筛选

###### 2.使用栏

![Filter](F:\vacation\gephi\img\Filter.png)



###### 3.使用逻辑

###### 4.呈现

### 三.Data Laboratory

### 四.Preview

##### 1.功能

做最后的美化，包括图形外观样式的选择，显示细节的调整。

##### 2.使用栏

预设置可选择渲染的一个大概的风格。

设置可以对节点，边，标签等进行参数的调整。

管理渲染器可以对渲染的顺序进行一个调整。

![preview](F:\vacation\gephi\img\preview.png)

##### 5.呈现

![preview2](F:\vacation\gephi\img\preview2.png)



### 五.Dynamic Data



### Extra

[力导向绘图 (Force-directed graph drawin]可以用于描述关系图的结点之间的关系，把结点分布到画布上合理的位置，比如描述企业之间的关系，社交网络中的人际关系等。



度，权值



思路：一个关于各种平台的网络关系（网络神经元）

导入数据

<img src="F:\vacation\gephi\img\1.png" style="zoom:50%;" />

<img src="F:\vacation\gephi\img\2.png" style="zoom:50%;" />

以度为标准区分节点的大小（以及标签）



<img src="F:\vacation\gephi\img\3.png" style="zoom:50%;" />

<img src="F:\vacation\gephi\img\5.png" style="zoom:50%;" />

通过样条曲线改变节点大小与度的关系

节点的度和节点的大小关系不应该成一个线性的关系，一般来说一个社区包含少数度较高的和一群的度较小的，那么应该将这种关系更加夸张地展示出来。（个人理解）

<img src="F:\vacation\gephi\img\4.png" style="zoom:50%;" />

根据Group的属性来进行一个分割，一般数据经过模块化的操作，也可以进行社区的划分

<img src="F:\vacation\gephi\img\6.png" style="zoom:50%;" />

加入一个力引导布局

<img src="F:\vacation\gephi\img\7.png" style="zoom:50%;" />





为了让数据更清晰的展示，能够展现出不同社区以及其相互关联，目标是想让同一个社区的各个节点能够比较紧密，而不同地社区能够保持一定的距离，主要是合理地调整引力和斥力的大小。

<img src="F:\vacation\gephi\img\8.png" style="zoom:50%;" />

最后在预览中做一个渲染

![](F:\vacation\gephi\img\9.png)

