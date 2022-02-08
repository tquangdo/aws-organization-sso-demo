# aws-organization-sso-demo 🐳

![Stars](https://img.shields.io/github/stars/tquangdo/aws-organization-sso-demo?color=f05340)
![Issues](https://img.shields.io/github/issues/tquangdo/aws-organization-sso-demo?color=f05340)
![Forks](https://img.shields.io/github/forks/tquangdo/aws-organization-sso-demo?color=f05340)
[![Report an issue](https://img.shields.io/badge/Support-Issues-green)](https://github.com/tquangdo/aws-organization-sso-demo/issues/new)

![overview](screenshots/overview.png)

## reference
[awsstudygroup](https://000012.awsstudygroup.com/vi)

## structure
- see on `AWS Organization`
![10](screenshots/10.png)
- see on `AWS SSO`
![5](screenshots/5.png)
### A) Permissions sets=`AdministratorAccess`
- OU=`Application Unit` > username=`Application` > groupname=`AWS-Application-Admin`
- OU=`Security Unit` > username=`Security` > groupname=`AWS-Security-Admin`
![9](screenshots/9.png)
### B) Permissions sets=`SecurityAudit`
- OU=`Logging Unit` > username=`Logging` > groupname=`AWS-Logging-Read-Only`
![2](screenshots/2.png)
---
![8](screenshots/8.png)
- lastly, after login by username=`Logging` (get PW by workaround way: click `Forgot PW`), at Dashboard can NOT access full services like the others!

## AWS SSO
![5](screenshots/5.png)
### A) Thêm Users và Groups
#### Users
- `Super-User` sẽ có quyền truy cập vào tất cả các group
![AddSuperUser](screenshots/AddSuperUser.png)
- after create `Super-User`:
![7](screenshots/7.png)
#### Groups
- 4 groups:
![6](screenshots/6.png)
### B) Tạo Permission Set
![per_set](screenshots/per_set.png)
### C) Gán quyền
![AssignUser](screenshots/AssignUser.png)
### check by Super-User
- after created will have login information
![superuser](screenshots/superuser.png)
- must change PW in 1st login
![NewPassword](screenshots/NewPassword.png)
- after login
![4](screenshots/4.png)
- click `Logging > Management console`
![3](screenshots/3.png)
- => can login SSO at username=`Logging` by `Super-User`. At top right corner: Federated user=`AWSReservedSSO_SecurityAudit_xxx`
- at Dashboard can access full services like `Super-User`

