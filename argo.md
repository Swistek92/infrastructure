<!-- quick start -->

kubectl create namespace argocd
kubectl apply -n argocd -f https://raw.githubusercontent.com/argoproj/argo-cd/stable/manifests/install.yaml

<!-- open port -->

kubectl -n argocd port-forward service/argocd-server 8080:80

<!-- initial credentials -->

login : admin

password:

kubectl get secret argocd-initial-admin-secret -n argocd -o yaml

<!--  decode password from base 64 -->

echo dmktY3p4NjlhUzZOSDFrTw== | base64 --decode
vi-czx69aS6NH1kO
qq
