Alternate OCP way
=================

```
cd shopfront/

mvn clean install

docker build -t mwitzenm/djshopfront:1.0 .

docker push mwitzenm/djshopfront:1.0

### IF you just want to build it from my image on docekerhub ###
oc apply -f ../kubernetes/shopfront-service.yaml
```
