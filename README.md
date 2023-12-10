# Introduction to helm and Installing-Helm

1. what is helm?
Helm is often referred to as the package manager for Kubernetes. It enables you to define, install, and manage even the most complex Kubernetes applications. Helm uses a packaging format called charts, which include all the resources needed to run an application, service, or a complete cloud-native stack inside Kubernetes.

# installing Helm
1. Get Signing key of helm
   ```bash
   curl https://baltocdn.com/helm/signing.asc | gpg --dearmor | sudo tee /usr/share/keyrings/helm.gpg > /dev/null
   sudo apt-get install apt-transport-https --yes
   echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/helm.gpg] https://baltocdn.com/helm/stable/debian/ all main" | sudo tee /etc/apt/sources.list.d/helm-stable-debian.list
   ```
2. Update Package manager ain install helm
   ```bash
   sudo apt-get update
   sudo apt-get install helm
   ```
 
