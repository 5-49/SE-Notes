# 3.1 通用过程模型

standard process??

![image-20210927104412103](C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210927104412103.png)

线性

迭代

![image-20210927105215302](C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210927105215302.png)

演化：迭代，螺旋上升

并行：comm和plan并行推进

# 3.2 定义框架活动

针对特定的问题，开发人员和利益相关者，哪些动作适合与框架活动？

例如communication activity中最重要的action打电话，包含的task set为

<img src="C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210927110008120.png" alt="image-20210927110008120" style="zoom: 50%;" />

3和4存在迭代

# 3.3 明确任务集

9.29 satrt

需要选择最能满足最适合开发团队特点的task set

下图是communication阶段的一个action：elicitation

![image-20210927112539850](C:\Users\eess6\AppData\Roaming\Typora\typora-user-images\image-20210927112539850.png)

7 用户场景：use case图

9 增量交付：第一次交付发现问题，再改进再次交付（迭代）

11 法律限制、权限限制

上面的步骤并不是线性的，是迭代进行的

**非功能需求：non-function**

1. **性能需求**

   算法，后台架构，数据库设计（冗余，将访问频率最高的表放在不同的table space里），微服务调用依赖关系，前后API接口，前端本身（要适当分担一些后端的任务）

2. **安全需求**

   加密方式？



coding这个activity的action：看成一个action

1. understand component design：理解详细设计
2. 找到核心复杂算法，定义数据结构，完成算法逻辑
3. 选择特定的IDE，并且实现代码
4. 自测试（做好了unit testing甚至可以裁掉）
5. 重构
6. SQA：software quality assurance 检查日志规范、接口、变量名
7. review：group review
8. code finish：0工作量





# 3.4 过程模式

本章最重要 process patterns

patterns：已证实有用的，抽象成一个模板步骤

代码变量不能用拼音

## Pattern name

名字，英语

## Force

所需要的实施环境，硬件，网络，版本管理工具

## Type

1. stage pattern ：解决和activity相关的
2. task pattern：指action或者task的
3. phase pattern：the sequence of framework activities



Initial Context：实施启动条件——之前的活动？进入状态？

Problem：这个模式能解决什么问题

Solution：如何实现？

Resulting Context：接口，就是一个出口条件，那些信息能够提交给接下来的

Related Pattern：

已知example：



prototype medol：帮助搞清需求













