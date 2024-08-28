## access alpine container
kubectl logs simple-multi-container-pod -c alpine-container

## Access container in pod (nginx)

kubectl exec -it simple-multi-container-pod -c nginx-container -- /bin/bash


## Kubectl command to taint a node

kubectl taint nodes ip-172-31-43-102.ap-south-1.compute.internal type=high:NoSchedule
kubectl taint nodes ip-172-31-5-29.ap-south-1.compute.internal type=high:NoSchedule
