# memcached-operator
### Operator SDK memcached-operator example

###### Operator Container Build and Push

make docker-build docker-push IMG=jamesjohnmoore/memcached-operator:1.0

cd config/default/ && kustomize edit set namespace "default" && cd ../..

make deploy IMG=jamesjohnmoore/memcached-operator:1.0

kubectl get deployment
