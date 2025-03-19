

#### IAM 사용자 password 변경
```
aws iam update-login-profile --user-name <username> --password <password>
```

#### 현재 사용자 정보 출력

```
aws sts get-caller-identity
```