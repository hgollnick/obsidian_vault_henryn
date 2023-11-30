
```
kubectl get pods -n a4t-3atool
kubectl logs -n a4t-3atool -f aaatool-060-deployment-64846c68db-c8q9n > /c/temp/3atool060.dev.log
kubectl exec -n a4t-gato -it gato-deployment-6b9c99b6ff-4bl56 bash
kubectl port-forward -n a4t-gato gato-deployment-79fd585b94-2xbd5 8787:8787