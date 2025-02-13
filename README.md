# civoK8s


Kubeconfig
 cp /Users/vansh/learn/Civo/civo-vanshpatel-kubeconfig  ~/.kube/config
 
kubectl Deployment
kubectl apply -f kubectl/
host change in ingress DNS



AgroCD: 

# Getting passwor for argoCD
kubectl get secret -n argocd argocd-initial-admin-secret -o jsonpath='{.data.password}' | base64 -d; echo                     

# port forwading at localhost:8080
kubectl port-forward svc/argo-cd-argocd-server -n argocd 8080:443

