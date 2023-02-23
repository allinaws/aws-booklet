**背景**

> 有个aws账号根用户绑定了MFA二次验证，但是不小心在手机上删除了此软件，导致了无法在登录aws控制台的时候无法输入二次验证吗，而此账号上面又没有其他IAM用户。

**过程**

先通过此链接的操作进行，发现不好使。
https://docs.aws.amazon.com/zh_cn/IAM/latest/UserGuide/id_credentials_mfa_lost-or-broken.html

再通过尝试进行找回或者跳过MFA设置
https: [//aws.amazon.com/blogs/s](https://aws.amazon.com/blogs/s) ecurity/ reset-your-aws-root-ac counts-lost-mfa-device-faster -by-using-the-aws-management- console/

1、我验证通过了第一步。邮箱和密码都是正确的。
2、第二步需要验证手机号，这里是需要接收电话语言。不知道什么原因我的手机 无法接受电话，
3、在这步骤上aws回给你回复邮件，直接在邮件上给aws交流，说手机号无法接收到语言验证码，**然后与aws约定某个时间进行通话验证**
4、约定时间，上来先确认名字和邮箱地址，然后会给你的邮箱发个一次性密码，你告诉aws工作人员后他会帮你删除MFA设置。
5、成功登录到aws控制台