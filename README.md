# YJCMS exist incorrect access control
1. ### Introduction to YJCMS

  YJcms is developed by gansu yunjing digital technology co., ltd. YJcms (Cloudscape cms) is an open source PHP enterprise website building management system developed based on ThinkPaPHP5.0.24. Yjcms adheres to the concept of minimalist, fast and extreme development, integrates enterprise, tourism and mall modules for development, and is a module and plug-in that can be easily and rapidly expanded. To facilitate developers to quickly build their own applications.

Address of the company's official website：[www.eyunjing.cn](http://www.eyunjing.cn/)

Test targets:

1.http://gszhjzx.com/user.html
2.http://lzrzjs.com/user.html

2. Vulnerability exploitation process

The homepage of the normal website is shown as follows

http://gszhjzx.com/

![image-20221109153216765](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20221109153216765.png)

> http://gszhjzx.com/index/user/user_edit.html
>
> Visit The Above Url

You can directly return the system user account and password without authentication information

![image-20221109153625703](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20221109153625703.png)

The password is MD5 encrypted, crack it

![image-20221109153651062](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20221109153651062.png)

![image-20221109153839089](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20221109153839089.png)

Let's visit this

http://gszhjzx.com/user_login.html

Enter the account password we obtained, in order to check whether the login can be successful

> Enter account: admin123 
>
> Password: admin123

You can see that the website was successfully logged in

![image-20221109154135043](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20221109154135043.png)
![image-20221109154342105](C:\Users\HP\AppData\Roaming\Typora\typora-user-images\image-20221109154342105.png)