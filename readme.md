# AWS GO SDK
![go-awesome](https://www.progville.com/wp-content/uploads/2015/01/aws-sdk-go-golang.jpg)

## List all IAM Users

### Requirements

Go SDK [installed and configured](https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/setting-up.html).  
AWS CLI Tool [installed and configured](https://docs.aws.amazon.com/cli/latest/userguide/installing.html) or AWS environment variables exported.

### Usage

**Run:**

`export AWS_PROFILE=myuser`

`go run main.go`


### Minimal IAM Policy

```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "awesome-minimal",
            "Effect": "Allow",
            "Action": "iam:ListUsers",
            "Resource": "*"
        }
    ]
}
```

**Output:**

```
[0] Username: golang               	 Created: 2018-01-25 05:53:58 +0000 UTC
[1] Username: jucknorris           	 Created: 2018-01-16 19:38:32 +0000 UTC
[2] Username: terra               	 Created: 2018-01-16 20:09:18 +0000 UTC
[3] Username: heidi                	 Created: 2018-01-25 02:04:27 +0000 UTC
[4] Username: lola                	 Created: 2018-01-25 02:05:21 +0000 UTC
```

### Links

- [Go Lang Doc](https://golang.org/doc/)
- [AWS SDK for Go](https://docs.aws.amazon.com/sdk-for-go/v1/developer-guide/welcome.html)

![go-awesome](http://www.qureet.com/blog/wp-content/uploads/2013/11/jumbo_gopher-4bf98fbc72cc188289ba2b458d4ce680.png)