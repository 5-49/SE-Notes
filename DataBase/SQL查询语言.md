# SQL简介

结构化查询语言Structured Query Language

如果不能为空可创建时候后缀not null

常用命令
```sql
insert into r values（ ， ， ）;
--将数据添加到关系中，括弧里的数据遵循在关系模式中列出的顺序
delete from r;--保留关系r，但删除r中的所有元组
drop table r;--不仅删除元组，还删除r的模式
alter table r add A D;
--为已有关系添加属性，A是待添加属性的名字，D为添加属性的域
alter table r drop A;--从关系中去掉属性
```

# SQL基本结构
## 单关系查询

```sql
--找出所有教师所在系名
SELECT dept_name
FROM instructor;

--强行删除重复
SELECT DISTINCT dept_name
FROM instructor;

--指明不删除重复
SELECT ALL dept_name
FROM instructor;

--用加减乘除+-*/来运算，显示给每位教师涨10%工资的结果
SELECT salary*1.1
FROM instructor;

--where子句，可以插入使用and，or，not
SELECT name
FROM instructor
WHERE dept_name='comp.sci'AND salary>7000;//注意不是==
```

## 多关系查询
```sql
--从多个关系中获取数据的查询
--找出教师姓名、系名、以及系的建筑名称
SELECT name,instructor,dept_name,buiding
FROM instructor,department
WHERE instructor.dept_name=department.dept_name;
```
运算顺序：
FROM, 在后面列出的关系产生笛卡尔积
WHERE, 在第一步骤的结果上应用WHERE的谓词
SELECT, 对步骤二的每个元组，选出SELECT的指定属性

## 自然连接
自然连接（natural join）运算作用于两个关系，并产生一个关系作为结果。它只考虑在两个关系模式中都出现的属性上取值相同的元组对。（共同属性相同）
```sql
--列出教师的名字以及他们所讲授课程的名称
SELECT name,title
FROM instructor NATURAL JOIN teaches, course
WHERE teaches.course_id=course.course_id

--不能这么写,这样会把“教的课不在自己的系”的老师忽略掉
SELECT name,title
FROM instructor NATURAL JOIN teaches NATURAL JOIN course

--using可以指明要自然连接的属性
SELECT name,title
FROM （instructor NATURAL JOIN teaches）JOIN course USING (course_id);
```

# 附加运算
## 更名运算
```sql
--更换名字用as语句，可以用在SELECT和FROM里
SELECT T.name, S.name
FROM instructor AS T,teaches AS S
WHERE T.ID=S.ID;
```
## 字符串运算
## select子句中的属性说明
## order by排列元组的显示次序
```sql
--最后加一句
ORDER BY a;
--可以使得SELECT的结果
ORDER BY a desc;
--desc表示降序，asc表示升序
```
