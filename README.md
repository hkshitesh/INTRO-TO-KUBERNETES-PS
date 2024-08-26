## access alpine container
kubectl logs simple-multi-container-pod -c alpine-container

## Access container in pod (nginx)

kubectl exec -it simple-multi-container-pod -c nginx-container -- /bin/bash
