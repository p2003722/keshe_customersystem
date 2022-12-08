# 客户消费积分管理系统

##### 写在前面

该项目是本人大二上学期课设，功能不是很全，有些许功能尚未完善，但主体结构完整，功能答题齐全，主要使用html和php语言，采用mysql数据库

##### 搭建方式

通过自己搭建web服务器访问，测试用环境为php8.0.25、mysql5.6.50

##### 主界面

![image](https://s1.ax1x.com/2022/12/09/zRmt5n.png)

在首次使用时会要求用户登录，以增强安全性。登录之后也可以进行登出操作。用户信息存储在表user中

![image](https://s1.ax1x.com/2022/12/09/zRmUCq.png)

进入主界面后，会自动加载整个用户表，并按照录入顺序（即自增id主键）进行排序。在用户详情中，通过用户的积分将用户分为五个等级（<10、1-99、100-999、1000-9999、>10000），并自动计算折扣率。在操作栏中，我们可以对客户进行编辑、积分、删除的操作。客户信息存储在表client中

##### 编辑界面

![image](https://s1.ax1x.com/2022/12/09/zRma80.png)

##### 积分界面

![image](https://s1.ax1x.com/2022/12/09/zRmd2V.png)

##### 删除提示框

![image](https://s1.ax1x.com/2022/12/09/zRmwvT.png)

### 同时有添加、搜索客户功能，并支持导入、导出

##### 添加界面

![image](https://s1.ax1x.com/2022/12/09/zRmBKU.png)

##### 搜索界面

在搜索界面我们引入了模糊搜索的功能，使得客户名字中有生僻字或者记不清楚完整手机号码时更加易于查找。查找同时在客户姓名和客户电话两栏中进行，更加方便快捷
在导出时我们采用了csv格式，相比于txt拥有更好的可读性

![image](https://s1.ax1x.com/2022/12/09/zRmDrF.png)

### 其他特色

##### 在添加、编辑界面我们使用正则表达式对手机号合法性进行验证，如果不合法会给出错误提示并返回

![image](https://s1.ax1x.com/2022/12/09/zRmrb4.png)

![image](https://s1.ax1x.com/2022/12/09/zRmyVJ.png)

在积分小于零时会给出提示

![image](https://s1.ax1x.com/2022/12/09/zRm6a9.png)
