# K8s-notes
Collection of notes on Kubernetes


## Kubectl

```shell
# delete pods by pattern matching
kubectl get pods -n ns-abc --no-headers=true | awk '/pod-name-prefix/{print $1}'| xargs  kubectl delete -n ns-abc pod

```
