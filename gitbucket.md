how to install gitbucket on pi 3

device : raspberry pi 3B+

download java 8 from 

download gitbucket from

https://github.com/gitbucket/gitbucket/releases

now you will have these ones

1. jdk-8-linux-arm-vfp-hflt.tar.gz
2. gitbucket.war

1. install java 8

make a shortcut for javac

```sudo tar zxvf jdk-8u181-linux-arm32-vfp-hflt.tar.gz -C /opt```
```sudo update-alternatives --config javac```

make a shortcut for java

```sudo update-alternatives --install /usr/bin/java java /opt/jdk1.8.0_181/bin/java 1```
```sudo update-alternatives --config java```

check 

```javac -version```
```java -version```

2. install gitbucket, sorry no install just run

```java -jar gitbucket.war```

3. login 

open http://raspberrypi.local:8080 or the pi.ip:8080

login as root(psk:root) 

enjoy


-------------- one more thing ----------------

if you need tomcat to run gitbucket 

here we go

download tomcat from https://tomcat.apache.org

if prefer tomcat 9 

https://tomcat.apache.org/download-90.cgi

click the core .tar.gz one

now we turn to pi

tar xvf tomcat.tar.gz

put war file into webapp

check pi.ip:8080/warname