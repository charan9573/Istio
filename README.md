# Istio installation
1  sudo apt install curl wget apt-transport-https -y
    2  sudo curl -fsSL https://get.docker.com -o get-docker.sh
    3  ll
    4  vim get-docker.sh
    5  sudo sh get-docker.sh
    6  sudo curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
    7  ll
    8  chmod +x minikube-linux-amd64
    9  ll
   10  sudo mv minikube-linux-amd64 /usr/local/bin/minikube
   11  ll
   12  minikube version
   13  sudo curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
   14  ll
   15  chmod +x kubectl
   16  ll
   17  sudo mv kubectl /usr/local/bin/kubectl
   18  ll
   19  kubectl version
   20  minikube version
   21  minikube start
   22  minikube start --driver=docker --force
   23  $ curl -L https://istio.io/downloadIstio | sh -
   24  curl -L https://istio.io/downloadIstio | sh -
   25  cd istio-1.23.0
   26  ls
   27  export PATH=$PWD/bin:$PATH
   28  ls bin
