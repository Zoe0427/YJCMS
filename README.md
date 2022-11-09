# YJCMS exist incorrect access control
1. ### Introduction to YJCMS

  YJcms is developed by gansu yunjing digital technology co., ltd. YJcms (Cloudscape cms) is an open source PHP enterprise website building management system developed based on ThinkPaPHP5.0.24. Yjcms adheres to the concept of minimalist, fast and extreme development, integrates enterprise, tourism and mall modules for development, and is a module and plug-in that can be easily and rapidly expanded. To facilitate developers to quickly build their own applications.

Address of the company's official website：[www.eyunjing.cn](http://www.eyunjing.cn/)

Test targets:

1.http://gszhjzx.com/user.html

2.http://lzrzjs.com/user.html

2. Vulnerability exploitation process

The homepage of the normal website is shown as follows

http://xxx.com/

![image](https://user-images.githubusercontent.com/75592724/200769402-ffab6db4-dbd6-4f59-af3e-3e67555abc2f.png)

> http://xxx.com/index/user/user_edit.html
>
> Visit The Above Url

You can directly return the system user account and password without authentication information

![image](https://user-images.githubusercontent.com/75592724/200770548-d83af410-a3ea-4706-bb40-05db36569032.png)

The password is MD5 encrypted, crack it

![image](https://user-images.githubusercontent.com/75592724/200769901-d5f2be73-15c6-46bd-b52a-7316cb53265e.png)

![image-20221109153839089](https://user-images.githubusercontent.com/75592724/200769762-49edd9b0-e9c5-49d2-a824-971ffabb1a45.png)

Let's visit this

http://xxx.com/user_login.html

Enter the account password we obtained, in order to check whether the login can be successful

> Enter account: admin123 
>
> Password: admin123

You can see that the website was successfully logged in

![image](https://user-images.githubusercontent.com/75592724/200770809-253bcd38-0a02-4b4d-90ad-b95b31c5df37.png)
![image](https://user-images.githubusercontent.com/75592724/200770917-b8128dda-325d-486e-add0-026c3d2182aa.png)
