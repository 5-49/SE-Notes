# Agile概念

适应需求、技术不断地变化

1. 看重团队结构、协作态度
2. 快速交付，不看重中间产品
3. 可使用非正式的开发方法，中间建模尽量简单
4. 和利益相关者在一个敏捷开发团队（命运共同体），roles、responsibility随时调整

![image-20211025103408928](ch5敏捷开发.assets/image-20211025103408928-16351292550421.png)

横坐标：开发过程中需求不断变化

虚线：需求变化控制在一个理想范围内

蓝色：上升的一个重要原因——regression testing回归测试（这一版和上一版本的修改会有牵连——相关用例）

5.3要看，会提问

# XP极限编程extreme programming

![image-20211025105239448](ch5敏捷开发.assets/image-20211025105239448.png)

适合比较大，周期长，风险高的项目

## planning

用户故事：这里story就是requirement，故事的单位unit是use case；

​	value：给故事划分优先级priority，选优先级高的在本次迭代实现

​	acceptance test：验收测试，主要看客户需求，需求归约。可以做测试用例的设	计（虽然还没code，但需求明确就可以做）

iteration plan：迭代计划关注两个方面——duration + mini-milestone

## design

**CRC**：class responsibility colabelraltor（协调者）‘

提取业务类：

抽象子系统：

类的方法和属性统称responsibility（用户的姓名生日）



类和其他类有交互叫：colaberator

1. 抽象子系统，抽象类负责交互（接口类）

例如我需要知道你的成绩，需要getGPA，那么我们俩就有协作关系。



九个类，三个子系统，互相之间可能有调用。

第一次要划分子系统

![image-20211027101703873](ch5敏捷开发.assets/image-20211027101703873.png)

每一次迭代需要把新增加的类的调用关系标记出来

最终得到软件的体系结构图（模块结构图）（一个树）《体系结构设计、数据库设计、接口设计》



非面向对象的架构：

<img src="ch5敏捷开发.assets/image-20211027101918803.png" alt="image-20211027101918803" style="zoom:33%;" />



Spike：某个算法特别复杂，应该拿出来做特定环境下的验证



## coding

团队不是直接开始code，而是先开发包含所有故事的单元测试

refactoring：自反，为了代码的质量

pair pro：结对编程，尤其是关键性的复用性高的项目。两个人一起写，一起查，一起review

continuous integration：集成测试，结对编程之后需要和团队其他人的集成起来

smoking testing：功能基本可以实现，最初来源于汽车行业（保证发动机冒烟）

## test

以类做单元测试，写一个脚本，把类放进去，直接等结果

continues inter：集成测试

# Scrum

适合迭代周期小的，最多4周。  

见pdf文档















