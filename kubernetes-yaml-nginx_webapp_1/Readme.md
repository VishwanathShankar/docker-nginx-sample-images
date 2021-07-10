Create a deployment yaml using the command
>kubectl create deployment nginx-webapp1 --image=vishwa787/webapp-1 --dry-run=client -o yaml > nginx-webapp1.yaml	

Test the deploymeny in K8s
> kubectl apply -f nginx-webapp1.yaml

Create a service for accessing the webapp
>kubectl create service nodeport nginx-webapp1-service --tcp=5678:80 --dry-run=client -o yaml
