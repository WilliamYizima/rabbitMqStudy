## To create cluster rabbitMQ in K8s

- Implement Operator:
```
kubectl apply -f https://github.com/rabbitmq/cluster-operator/releases/latest/download/cluster-operator.yml
```

- Implement configmap of RabbtiMq:
```
kubectl apply -f k8s/rabbitmq.yaml
```