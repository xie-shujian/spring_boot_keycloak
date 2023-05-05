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
