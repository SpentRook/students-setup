# Kubernetes Deployment with kubectl

This markdown file explains the steps to create a deployment in Kubernetes using the `kubectl` command-line tool.

## Step 1: Create a Deployment

To create a deployment named `api` with the image `danielsabana/k8sexample:1.0.0` and expose port `8080`, run the following command:


generate a md explaning the following steps:

kubectl create deployment api --image=danielsabana/k8sexample:1.0.0 --port=8080

kubectl get pods    

kubectl describe pod api-65cdfb94f-5x44x


other way: 

kubectl create deployment api --image=danielsabana/k8sexample:1.0.0 --port=8080 --dry-run=client -o yaml >api-deployment.yaml