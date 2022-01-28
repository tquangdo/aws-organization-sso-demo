# aws-organization-sso-demo 🐳

![Stars](https://img.shields.io/github/stars/tquangdo/aws-organization-sso-demo?color=f05340)
![Issues](https://img.shields.io/github/issues/tquangdo/aws-organization-sso-demo?color=f05340)
![Forks](https://img.shields.io/github/forks/tquangdo/aws-organization-sso-demo?color=f05340)
[![Report an issue](https://img.shields.io/badge/Support-Issues-green)](https://github.com/tquangdo/aws-organization-sso-demo/issues/new)

![overview](screenshots/overview.png)

## reference
[awsstudygroup](https://000012.awsstudygroup.com/vi)

## 4 groups
![6](screenshots/6.png)

## structure
- see on `AWS Organization`
![10](screenshots/10.png)
- see on `AWS SSO`
![5](screenshots/5.png)
### A) Permissions sets=`AdministratorAccess`
- OU=`Application Unit` > username=`Application` > groupname=`AWS-Application-Admin`
![1](screenshots/1.png)
- OU=`Security Unit` > username=`Security` > groupname=`AWS-Security-Admin`
![9](screenshots/9.png)
### A) Permissions sets=`SecurityAudit`
- OU=`Logging Unit` > username=`Logging` > groupname=`AWS-Logging-Read-Only`
![2](screenshots/2.png)
---
![8](screenshots/8.png)
- => after login by username=`Logging`, can NOT access full like the others!

## Super-User
- [create](https://000012.awsstudygroup.com/vi/2-setup-aws-sso/2.2-add-user-group/)
![7](screenshots/7.png)
- after created will have login information
![superuser](screenshots/superuser.png)
- after login
![4](screenshots/4.png)
- click `Logging > Management console`
![3](screenshots/3.png)

