## Educational Schema
``
Deploy app
``

```
kubectl -n <NAMESPACE> create secret generic  schema-config --from-file=Common.json --from-file=Address.json --from-file=Institute.json --from-file=Student.json --from-file=Teacher.json

kubectl -n <NAMESPACE> apply -f registry-deployment.yaml

kubectl -n <NAMESPACE> apply -f claim-ms-deployment.yaml

```
