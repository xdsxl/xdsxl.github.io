### 试论述类与用例的区别。 
答：（1）联系：用例图与类图都是一种半形式化的语言，相较于自然语言，它们更加严谨、易懂，便于沟通。
（2）区别：用例图主要是面向用户描述系统功能，并指出各功能的操作者。主要用于需求分析时详细了解用户的需求，获得更全面、精准的用户需求；类图则是主要面向程序设计者的，用于项目的细分，便于程序员之间的交流，也能够有效地进行工作分配。

### 试比较边界类与实体类的异同。
答：（1）实体类是对系统中需要存储的信息和其信息的行为建立模型。实体类具有永久的特性，这类似于数据库中的表一样用于保存系统的业务信息。
    （2）边界类位于系统与外界的交接处，它在一个或多个角色和系统之间建立相互作用的模型。
### 2.4    
### 学期筛选类：
### 属性：
         全部数据             类型为String，Private属性
	18至19学年上学期	类型为String，Private属性
	18至19学年下学期	类型为String，Private属性
	19至20学年上学期	类型为String，Private属性
	19至20学年下学期	类型为String，Private属性
### 方法：	
  查询	
  打印	

### 成绩下载类：
### 属性：	
  姓名	类型为String，Private属性
	学号	类型为int，Private属性
	学院	类型为String，Private属性
	班级	类型为String，Private属性
	学期	类型为String，Private属性
	课程名称	类型为String，Private属性
	课程性质	类型为String，Private属性
	成绩类型	类型为String，Private属性
	应修学分	类型为String，Private属性
	实修学分	类型为String，Private属性
	成绩	类型为String，Private属性
	绩点  	类型为String，Private属性
	学分绩	类型为String，Private属性
### 方法：	
  保存	
	发送	

### 成绩类
### 属性	
  考试科目	类型为String，Private属性
	总评成绩	类型为String，Private属性
	学期	    类型为String，Private属性
	学科类型	类型为String，Private属性
	应修学分	类型为String，Private属性
	实修学分	类型为String，Private属性
	绩点	    类型为String，Private属性
	学分绩	   类型为String，Private属性
	平时成绩	类型为Int，Private属性
	作业成绩	类型为Int，Private属性
	期中成绩	类型为Int，Private属性
	期末成绩	类型为Int，Private属性
### 方法：	

### 教师参与者的类图
### 属性：
用户名: string
密码: string
所授学科: string
性别: string
### 方法：
上传课件
上传教学视频
发布教学心得
查看教学心得
修改教学心得
找回密码


