# Services Activities

## ClusterIP

```sh
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

kubectl get pods -o wide
kubectl get services -o wide

# create a route from your local machine to the K8s service running inside your cluster
kubectl port-forward service/k8s-intro-server-svc 4000:4000
```

Now open your browser to `http://localhost:4000` and verify that the page loads.
You should see a web page with the message "Welcome to Kubernetes!".

