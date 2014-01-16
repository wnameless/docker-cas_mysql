docker-mysql_phpmyadmin
============================

```
docker pull wnameless/cas-mysql
```

Run with 22, 80, 8080, 8443 and 3306 ports opened:
```
docker run -d -p 49160:22 -p 49161:80 -p 49162:8080 -p 49163:8443 -p 49164:3306 wnameless/cas-mysql
```

Login the CAS server https://localhost:49163/cas/login with following credential:
```
username: guest
password: guest
```
It's just a demo account. You can create more account by phpMyAdmin.
Be aware that all passwords suppose to be hashed by MD5.

Open http://localhost:49161/phpmyadmin in your browser with following credential:
```
username: root
password:
```

Open Tomcat web admin http://localhost:49162/manager/html with following credential:
```
username: admin
password: admin
```

Login by SSH
```
ssh root@localhost -p 49160
password: admin
```
