# Kubernetes
# Steps to install MINIKUBE INSTALLATION
1.Create one ubuntu instance in t3 medium
2.Connect the instance to the server
3.go the root user by the cmd sudo su -
4.Update the server by the command apt update -y
# install docker by the belown commands
sudo apt install curl wget apt-transport-https -y
sudo curl -fsSL https://get.docker.com -o get-docker.sh
chmod 777 get-docker.sh
sh get-docker.sudo h
# install  minikube by the belown commands
sudo curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo mv minikube-linux-amd64 /usr/local/bin/minikube
sudo chmod +x /usr/local/bin/minikube
sudo minikube version
# install kubectl by the belown commands
sudo curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
sudo curl -LO "https://dl.k8s.io/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl.sha256"
sudo echo "$(cat kubectl.sha256) kubectl" | sha256sum --check
sudo install -o root -g root -m 0755 kubectl/usr/local/bin/kubect
sudo install -o root -g root -m 0755 kubectl/usr/local/bin/kubectl
sudo kubectl version --client --output=yaml
sudo minikube start --driver=docker --force
kubectl run pod-name --image=image-name
Create the yaml file by the command vi file-name.yml
Write the script in the yml editor![Screenshot 2024-11-14 164445](https://github.com/user-attachments/assets/82b459ae-960b-4120-81ef-f6efa576c677)
Kubectl create -f filename.yml - by this command if pod is created then the work is done
Kubectl get pods – it is used to see the created pods as shown in below figure
![Screenshot 2024-11-14 172232](https://github.com/user-attachments/assets/f3543d17-3411-4578-8b29-a9679e630eac)


