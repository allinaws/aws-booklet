

创建此策略，并附加给iam用户

只允许此IP地址的请求访问aws控制台

```json
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "VisualEditor0",
            "Effect": "Allow",
            "Action": "*",
            "Resource": "*",
            "Condition": {
                "ForAnyValue:IpAddress": {
                    "aws:SourceIp": [
                        "111.222.333.444/32",
                        "ip-range"
                    ]
                },
            }
        }
    ]
}
```



根用户是你创建 AWS 账户时使用的邮箱地址和密码，它拥有完全的访问权限，不能被限制或附加任何策略。

你应该避免使用根用户进行日常任务，而是创建 IAM 用户并给予适当的权限。根用户是你创建 AWS 账户时使用的邮箱地址和密码，它拥有完全的访问权限，不能被限制或附加任何策略。你应该避免使用根用户进行日常任务，而是创建 IAM 用户并给予适当的权限。