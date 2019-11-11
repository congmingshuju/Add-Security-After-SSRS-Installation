![Lee Songming](https://github.com/congmingshuju/git-resources/blob/master/images/0-clever-data-github.jpg "李聪明 数据")


# SSRS安装后配置安全性
**Add Security After SSRS Installation**
**发布-日期:  2015年4月15日 (评论)**

## Contents

- [中文](#中文)
- [English](#English)
- [SQL-Logic](#Logic)
- [Build Quality](#Build-Quality)
- [Author](#Author)
- [License](#License) 


## 中文
当你安装并配置SSRS 2012后，你应该做的最重要的事情之一是为SSRS配置安全性。默认情况下，所有组都基本上被降级为普通用户（无论你是否已被添加为管理员）。UAC将始终阻止想要通过SSRS添加/创建/编辑报告的用户或应用程序的访问。解决方案很简单，只需要在报告服务中配置安全性来添加BuiltinAdministrators（或管理员在本地服务器上的其他组）。这是操作过程演示。
从已安装SQL Server Reporting Services的数据库服务器。

使用管理员权限打开浏览器。


## English
Once you have SSRS 2012 installed, and configured, one of the most important things you should do is configure security for SSRS. By default all groups are essentially relegated as a basic user (regardless if you have been added as admin or not). UAC will always block access to users or applications trying to add/create/edit reports via SSRS. The solution is to simply configure security within reporting services to add the BuiltinAdministrators (or other group the admins are a part of locally on the server). Here is the process for that.
From the database server where you have installed SQL Server Reporting Services.

Open the browser with Administrative rights.

* 1
![步骤1 (Step1)](images/step-1.jpg?raw=true "步骤1")

Go to this address:
http://MyServerName/Reports_MyInstanceName
Click Site Settings link on the right.

* 2
![步骤2 (Step2)](images/step-2.jpg?raw=true "步骤2")

Click the Security button on the left.

- 3
![步骤3 (Step3)](images/step-3.jpg?raw=true "步骤3")

Check the box next to BUILTINAdministrators, and click ‘Edit’.

- 4
![步骤4 (Step4)](images/step-4.jpg?raw=true "步骤4")

Select ‘System User’, and click ‘Apply’.

- 5
![步骤5 (Step4)](images/step-5.jpg?raw=true "步骤5")

你做好了 (You're done)



