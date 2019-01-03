product-catalogue
=================
```
java -jar target/product-1.0-SNAPSHOT.jar server product-catalogue.yml

docker build -t danielbryantuk/product .
docker run -p 9010:9010 -p 9011:9011 -d danielbryantuk/product
```

Alternate OCP way
=================
```
cd productcatalogue/

mvn clean install

docker build -t mwitzenm/djproductcatalogue:1.0 .

docker push mwitzenm/djproductcatalogue:1.0

### IF you just want to build it from my image on docekerhub ###
oc apply -f ../kubernetes/productcatalogue-service.yaml
```
