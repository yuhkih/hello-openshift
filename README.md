# hello-openshift  
Nginx test container based on UBI8

## How to build
```
docker build . -t hello-openshift:latest 
```

## How to use
```
$ docker run --rm --name hello-test -p 80:8080 -d hello-openshift:latest
$ curl http://localhost 
Hello OpenShift!
$ docker stop hello-test
```

