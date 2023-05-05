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
