﻿### MySQL修改root用户密码

#### 方法1： 用SET PASSWORD命令

```
mysql -u root　　
mysql> SET PASSWORD FOR 'root'@'localhost' = PASSWORD('newpass');
```

#### 方法2：用mysqladmin　　

```
mysqladmin -u root password "newpass"
```

如果root已经设置过密码，采用如下方法　　

```
mysqladmin -u root password oldpass "newpass"
```

#### 方法3： 用UPDATE直接编辑user表　　

```
mysql> UPDATE user SET Password = PASSWORD('newpass') WHERE user = 'root';　　
mysql> FLUSH PRIVILEGES;
```

在丢失root密码的时候，可以这样　　

```mysqld_safe --skip-grant-tables&　　
mysql -u root mysql　　
mysql> UPDATE user SET password=PASSWORD("new password") WHERE user='root';　　
mysql> FLUSH PRIVILEGES;
```
#### testing测试
#### 方法3： 用UPDATE直接编辑user表　　