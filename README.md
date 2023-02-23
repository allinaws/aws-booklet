all in aws



1、注册账号

2、登录后创建一个iam用户、并把根用户

* 密码修改为21+随机字符串
* 二次登录认证  [AWS 用户启用MFA](aws-mfa.md)
* 限制IAM用户登陆地  [限制访问地址](aws-allow-ip.md)

3、设置aws account别名 [AWS 设置账户ID别名](aws-account-alias.md)

4、把根用户账号密码给另一个不长操作aws的人

5、运维操作通过新创建的iam进行管理账号  [创建IAM用户](aws-iam-user.md)

