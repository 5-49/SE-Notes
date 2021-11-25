由此开始第二部分

第七章是总结起来最难的，都是概念

7、概念

8、9、10、11：requirement engeerning

8：requirement elistation

9、10、11：requirement analysis modeling



建模的目的：为了抽象，帮助理解，最终目的是为了方便coding



These software engineering principles are likely to serve a professional programmer throughout his or her career.

# Core Principles

## Principles That Guide Process

① Principle 1. Be agile.

② Principle 2. Focus on quality at every step.
每一次向product owner展示的时候就是在评价质量（每一大轮）
每一小轮也要注重质量
每一步都要通过评审、演示、评估管理质量

③ Principle 3. Be ready to adapt.
可以适应

④ Principle 4. Build an effective team.

⑤Principle 5. Establish mechanisms for communication and coordination.
团队内部沟通协调机制

⑥Principle 6. Manage change.
管理变更

⑦Principle 7. Assess risk.

⑧Principle 8. Create work products that provide value for others.
例如总结pattern

##  Principles That Guide Practice
①Principle 1. Divide and conquer.
分而治之，划分子系统

② Principle 2. Understand the use of abstraction.
activity功能逻辑的抽象，类图是数据角度的图像，use case是对产品对用户使用产品的抽象——一个use case是一个功能单元。
所有的建模都是抽象

swim也是activity diagram，只不过标记了有哪些类需要协作。
sequence

https://blog.csdn.net/wordwarwordwar/article/details/90233903

③Principle 3. Strive for consistency.
保持一致，不能出现偏差和矛盾

④Principle 4. Focus on the transfer of information.
输入输出就是信息转换的过程

⑤Principle 5. Build software that exhibits effective modularity.

⑥Principle 6. Look for patterns.

⑦Principle 7. When possible, represent the problem and itssolution from a number of different perspectives.

⑧Principle 8. Remember that someone will maintain the software.



# 每个activity的原则

## 7.3.1 Communication

①Principle 1. Listen.

②Principle 2. Prepare before you communicate.
有备而听，不然不了解行业内容会听不懂

③Principle 3. Someone should facilitate the activity.
有协调人安排会面等

④Principle 4. Face-to-face communication is best.

⑤Principle 5. Take notes and document decisions.

⑥Principle 6. Strive for collaboration.

⑦Principle 7. Stay focused; modularize your discussion.

⑧Principle 8. If something is unclear, draw a picture.
⑨Principle 9. ( a) Once you agree to something, move on. (b) If
you can't agree to something, move on. (c) If a feature or
function is unclear and cannot be clarifified at the moment,
move on.
⑩Principle 10. Negotiation is not a contest or a game. It works
best when both parties win.

## 7.3.2 Planning

①Principle 1. Understand the scope and boundry of the project.

②Principle 2. Involve stakeholders in the planning activity.

③Principle 3. Recognize that planning is iterative.

④Principle 4. Estimate based on what you know. 估算工作量

⑤Principle 5. Consider risk as you define the plan. 评估风险

⑥Principle 6. Be realistic. 实事求是

⑦Principle 7. Adjust granularity as you define the plan. 调整项目计划的粒度

⑧Principle 8. Define how you intend to ensure quality. 指定计划的时候也要确保质量

⑨Principle 9. Describe how you intend to accommodate change.

⑩Principle 10. Track the plan frequently and make adjustments as
required.



## 7.3.3 Modeling

depicting the software in three different domains:

 the information domain，数据建模，主要是类图

 the functional domain, 功能建模，活动图

and the behavioral domain. Design，行为建模，状态图

讲到ppt11页了，记得补充笔记

> requirement elistation
> requirement analysis modeling
> 这两个在一起是需求工程requirement engeering

① Principle 1. The primary goal of the software team is to build software, not create models. 

② Principle 2. Travel light—don’t create more models than you need. 

③ Principle 3. Strive to produce the simplest model that will describe the problem or the software. 

④ Principle 4. Build models in a way that makes them amenable to change.

⑤ Principle 5. Be able to state an explicit purpose for each model that is created. 

⑥ Principle 6. Adapt the models you develop to the system at hand. 

⑦ Principle 7. Try to build useful models, but forget about building perfect models. 

⑧ Principle 8. Don’t become dogmatic about the syntax of the model. If it communicates content successfully, representation is secondary. 

⑨ Principle 9. If your instincts tell you a model isn’t right even though it seems okay on paper, you probably have reason to be concerned. 

⑩ Principle 10. Get feedback as soon as you can.



需求分析建模：

① Principle 1. The information domain of a problem must be represented and understood.创建类图

 ② Principle 2. The functions that the software performs must be defined. 功能建模

③ Principle 3. The behavior of the software (as a consequence of external events) must be represented.行为建模

④ Principle 4. The models that depict information, function, and behavior must be partitioned in a manner that uncovers detail in a layered (or hierarchical) fashion. 不断细化

⑤ Principle 5. The analysis task should move from essential information toward implementation detail.



设计建模：

① Principle 1. Design should be traceable to the requirements model. 设计是以需求为依据的（V-model有体现）

② Principle 2. Always consider the architecture of the system to be built. 架构设计非常非常重要

③ Principle 3. Design of data is as important as design of processing functions. 数据设计也很重要：数据库，数据字典，数据结构，数据仓库

>数据字典：数据的组成方式。例如某个接口输入数据如何对应（送给）后台（类的某个属性/字符串）。也是界面设计的重要基础。

④ Principle 4. Interfaces (both internal and external) must be designed with care. 接口设计

⑤ Principle 5. User interface design should be tuned to the needs of the end user. However, in every case, it should stress ease of use. 

⑥ Principle 6. Component-level design should be functionally independent .高内聚

⑦ Principle 7. Components should be loosely coupled to one another and to the external environment . 低耦合

> 方法之间互相调用的时候参数尽量少

⑧ Principle 8. Design representations (models) should be easily understandable. 好理解

⑨ Principle 9. The design should be developed iteratively . 迭代

⑩ Principle 10. Creation of a design model does not preclude an agile approach

## 7.3.4 Construction

**Coding Principles:**

Constrain your algorithms by following structured programming practice.

 Consider the use of pair programming. 

Select data structures that will meet the needs of the design.

Understand the software architecture and create interfaces that are consistent with it.
写代码的时候注意类与类之间的关系，有接口就要增加方法。

Keep conditional logic as simple as possible. 
避免循环/if嵌套

Create nested loops in a way that makes them easily testable.  好测试

Select meaningful variable names and follow other local coding standards. 

Write code that is self-documenting. 加注释

Create a visual layout (e.g., indentation and blank lines) that aids understanding.

**Validation Principles**

Conduct a code walkthrough（走查，一种评审的方式，仅仅对代码） when appropriate.

Perform unit tests and correct errors you’ve uncovered. 
IDE继承单元测试，直接运行测试用例。

Refactor the code.代码重构。

> 可以在以下面对代码进行重构： 
>
> 1.重命名：对类，接口，方法，属性等重命名，以使得更易理解
>
>  2.抽取代码：将方法内的一段代码抽取为另一个方法，以使得该段代码可以被其他 方法调用，这是重构中很重要很常用的，此举可以极大的精炼代码，减少方法的 代码行数 
>
> 3.封装字段：将类的某个字段转换成属性，可以更加合理的控制字段的访问 （类如银行的分局号也为一个属性，卡号是另一个属性，用户只访问卡号）
>
> 4.抽取接口：将类的某些属性，方法抽取组成个接口，该类自动实现该接口
>
>  5.提升方法内的局部变量为方法的参数：这主要是在写代码的过程中会使用到 
>
> 6.删除参数：将方法的一个或多个参数删掉 
>
> 7.重排参数：将方法的参数顺序重新排列



**Testing principles**

①Principle 1. All tests should be traceable to customer requirements. 为了满足用户需求

②Principle 2. Tests should be planned long before testing begins 尽早做

③ Principle 3. The Pareto principle applies to software testing. 82规则

④ Principle 4. Testing should begin “in the small” and progress toward testing “in the large.” 

⑤ Principle 5. Exhaustive testing is not possible. 
穷尽测试是不可能的。

⑥ Principle 6. Apply to each module in the system a testing effort commensurate with its expected **fault density.** 

⑦ Principle 7. Static testing techniques can yield high results. 静态测试，代码走查

⑧ Principle 8. Track defects and look for patterns in defects uncovered by testing. 跟踪缺陷，找找有没有通用的方法解决

⑨ Principle 9. Include test cases that demonstrate software is behaving correctly.利用状态图（行为建模）设计测试

# WORK PRACTICES

接口，规范&模板，层次化，算法效率，哈希表，云平台，合理的数据库

