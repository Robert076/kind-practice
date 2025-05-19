# kind-practice

1. Create the pod:
```bash
kubectl apply -f nginx-pod.yml
```

2. Expose it to the web:
```bash
kubectl port-forward pod/nginx-pod 8080:80
```

3. Now access it by going to localhost:8080

---

### Extra *helpful* commands

1. Return the pods in your cluster in a json format:
```bash
kubectl get pods -o json
```

2. Return the pods in yoru cluster in a yaml format:
```bash
kubectl get pods -o yaml
```

3. Return the pods alongside their working node:
```bash
kubectl get pods -o wide
```

4. More detailed information about the pod:
```bash
kubectl describe pod/nginx-pod
```


