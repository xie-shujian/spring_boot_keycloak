# spring_boot_keycloak
# install keycloak
## download
https://www.keycloak.org/downloads.html
## keycloak version
21.1.1
## start in windows
bin/kc.bat start-dev
## need jdk 11
when you run java -version, get jdk1.8, then you need to add one line in **kc.bat**
```
set JAVA_HOME=C:\xxxx\jdk-11.0.12
```
## Open http://localhost:8080/
create the admin user and password
## login http://localhost:8080/admin/master/console/
## create test realm
![image](https://user-images.githubusercontent.com/1661052/236424081-fff85f3a-abeb-4370-977a-6fcaa3db9648.png)
## use the test realm
## create client id
test
## set client authentication to off
off is public access, on is oidc
## set redirect url to http://localhost:8081/*
## set home url to http://localhost:8081
## create two roles
test-role and user-role
## create user user1 and user2 and set password
## role map
map user-role to user1 and test-role to user2
# case 1
## create client testkeycloak
## Set Valid redirect URIs to https://www.keycloak.org/app/*
## Set Web origins to https://www.keycloak.org
## open https://www.keycloak.org/app/
change realm to test, client id to restkeycloak
## sign in with user1 or urser2
# case 2
## refer
https://blog.csdn.net/weixin_36380516/article/details/128731825
