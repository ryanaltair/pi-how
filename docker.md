install docker

Best way is __curl -sSL https://get.docker.com | sh__

switch as root
``` su root ```

run this
```curl -sSL https://get.docker.com | sh```

add pi to docker user group 
```sudo usermod -aG docker pi```

then you will get rid of ```sudo```

check with

```docker --version```