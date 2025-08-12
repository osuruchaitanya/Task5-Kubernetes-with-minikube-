# 🌐 Kubernetes App Deployment using Minikube

## 📖 Project Summary
This project demonstrates how to deploy and expose an application in a *local Kubernetes cluster* using Minikube.  
It covers cluster setup, YAML manifests, scaling, and dashboard monitoring.

---

## 🗂 Repository Structure

. ├── deployment.yaml      # Deployment configuration ├── service.yaml         # Service configuration ├── screenshots/         # Proof of setup & running app └── README.md            # Project documentation

---

## 🚀 Steps Performed

1. *Start Minikube*
   ```bash
   minikube start --driver=docker

2. Deploy the Application

kubectl apply -f deployment.yaml
kubectl apply -f service.yaml


3. Check Status

kubectl get pods -o wide
kubectl get svc


4. Access the Application

minikube service my-service


5. Scale Deployment

kubectl scale deployment my-deployment --replicas=5


6. Open Dashboard

minikube dashboard




---

📸 Screenshots
 
## Workload status:
![image alt](https://github.com/osuruchaitanya/Task5-Kubernetes-with-minikube-/blob/5d6dbf61b94c97d4248227189827994dcfa8af10/kubectl_workload.png)

## Pods  :
![image alt](https://github.com/osuruchaitanya/Task5-Kubernetes-with-minikube-/blob/63f6cc12152cb521b38b34fb7b6bff1780833d28/kubectl_get_pods.png)
![image alt](https://github.com/osuruchaitanya/Task5-Kubernetes-with-minikube-/blob/ec85832ba1da01258ff00534e996cdbebe0fe72c/kubectl_get_pods-1.png)
### service :
![image alt](https://github.com/osuruchaitanya/Task5-Kubernetes-with-minikube-/blob/c016dca524a46bc14a72324229147a7dc57c5d6c/kubectl_getsvc_svc.png)
![image alt](https://github.com/osuruchaitanya/Task5-Kubernetes-with-minikube-/blob/c5f69258e3c7796f99826e9fe307976b9ea877d4/kubectl_getsvc_svc1.png)
## Application running in browser:
![image alt](https://github.com/osuruchaitanya/Task5-Kubernetes-with-minikube-/blob/a86afd3321997d48959e50ce0637c3d34c0a88f8/output.png)


---

🛠 Tools & Technologies

Kubernetes

Minikube

kubectl

Docker



---

📌 Notes

Service type used: NodePort

Deployment image: nginx:stable (can be replaced with custom image)

Built and tested on local environment
