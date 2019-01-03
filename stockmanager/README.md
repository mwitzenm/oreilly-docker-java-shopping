Alternate OCP way
=================

```
cd stockmanager/

mvn clean install

docker build -t mwitzenm/djstockmanager:1.0 .

docker push mwitzenm/djstockmanager:1.0

oc apply -f ../kubernetes/stockmanager-service.yaml
```
