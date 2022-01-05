# 2.1 软件工程定义

![image-20210915112145009](C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210915112145009.png)

![image-20210915113258318](C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210915113258318.png)

sequence图是在use case上细化



CASE：计算机辅助软件工程

# 2.2 软件过程

一个activity由一个或多个actin构成，action又由多个任务构成。

interface+data

activity：

action：实现宽泛的目标

task：



milestone：两个activity的交付点，前一阶段的action已经检测无误，交付到下一阶段。本阶段的产品已经review了。

## 过程框架







## 普适性活动

risk exposure= loss* possibility

1. 识别风险
2. 计算risk exposure = loss* possibility（概率和损失的乘积）并排序
3. 根据第二步指定的策略实施，动态跟踪风险



## 过程框架

- 对一个preocess要不断分解：activity，action，task
- 为了更好地理解sfw pro——分解为两个维度：pro（制造）+um（保护）

提问过：

1. comunication：requirement modeling

2. Planing：umbrella 

3. Modeling：archtecture & componet desgin

4. Construction：coding & testing

5. Deployment：dilivery & mantainance & feedback

   

   软件开发过程包括很多迭代，并不是线性顺序的模型，而是循环往复。

里面包含什么归约？？？、、



## 普适性活动Umbrella activity***

导致changing的三个原因：提问过

1. correct纠错
2. 适应性修改：法律 adapt
3. enhance：增加性能，功能增强

SQA：查询接口监控

**测量Measurement：**





**可复用管理Reusability management：**例如java底层是跨平台的。再例如做银行开发，这个银行和另一个是一样的——做标准类库，标准接口。refactor重构的目的之一就是标准化。





## 过程的适应性调整

软件工程过程并不是教条的，而应该是灵活可适应的。可根据项目特点，组织文化等进行适应性调整。

![image-20210926100351370](C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210926100351370.png)





# 2.3 软件工程实践

9.26 start

## 实践的精髓

1. **理解问题：**利益相关者（stackholder），功能特性，是否可以划分
2. **策划解决问题：**是否已有解决方法/设计模式可以复用，修改；是否可以划分子问题
3. **实施计划：**
4. **检查结果的正确性：**vailidate？合理？单元测试后做系统测试（是否符合客户需求）



需求工程：

需求归约，文字描述需求---》use case（从用户角度的抽象）

class（数据建模的抽象），activity，state diagram，sequence（动态抽象）

component design：类的设计，有什么类，什么方法，继承关系——复杂的方法用activity diagram画出来



状态图（Statechart Diagram）主要用于描述一个对象在其生存期间的动态行为，表现为一个对象所经历的状态序列，引起状态转移的事件（Event），以及因状态转移而伴随的动作（Action）。——**是软件体系架构的依据。**

由状态图考虑要有什么类，怎样互相架构——**是类设计的重要依据。**

## 通用原则

1. 存在价值
2. 保持简洁
3. 保持愿景
4. 关注使用者
5. 面向未来
6. **提前计划复用**：前瞻性，降低成本
7. 认真思考

9.27 start

# 2.4 软件开发神话

management myth

1. 即使有软件工程这个开发框架也可能会遇到很多问题



customer myth

1. 需求不能随意更改，敏捷开发中需要等到下一个迭代周期才可以更改需求（stories）



Practitioner’s myths

1. 代码要写的慢而精
2. review SOA去找error
3. Software engineering is not about creating documents. It is about creating a quality product.



项目过程中尽量用开源工具

需求管理工具：

测试工具：

outsource

# 2.5 如何开始

