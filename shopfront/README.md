Alternate OCP way
=================

```
cd shopfront/

mvn clean install

docker build -t mwitzenm/djshopfront:1.0 .

docker push mwitzenm/djshopfront:1.0

### IF you just want to build it from my image on docekerhub ###
oc apply -f ../kubernetes/shopfront-service.yaml

### OR if you just want to run it without git clone ###
oc apply -f https://raw.githubusercontent.com/mwitzenm/oreilly-docker-java-shopping/master/kubernetes/shopfront-service.yaml

oc expose service shopfront
```
