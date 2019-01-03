Alternate OCP way
=================

```
cd shopfront/

mvn clean install

docker build -t mwitzenm/djshopfront:1.0 .

docker push mwitzenm/djshopfront:1.0

oc apply -f ../kubernetes/shopfront-service.yaml
```
