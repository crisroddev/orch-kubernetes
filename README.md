# Install Kubernetes
## Mac
`curl -LO "https://storage.googleapis.com/kubernetes-release/release/$(curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt)/bin/darwin/amd64/kubectl"`

## Linux 
`curl -LO https://storage.googleapis.com/kubernetes-release/release/`curl -s https://storage.googleapis.com/kubernetes-release/release/stable.txt`/bin/linux/amd64/kubectl`
 ## Features CPU
 sysctl -a | grep machdep.cpu.features
 sysctl -a | grep machdep.cpu.features | grep VMX

 ## Install Minikube
 `brew cask install minikube`

 ## Minikube Start
 `minikube start`

 # Cluster Info
 `kubectl cluster-info`

 # Get Nodes
 `kubectl get nodes`

 # Kubernetes Monitoring and Logging
 `wget https://github.com/prometheus/prometheus/releases/download/v2.27.0/prometheus-2.27.0.linux-amd64.tar.gz`
 `tar xvfz prometheus-2.27.0.linux-amd64.tar.gz`
 `prometheus --config-file=prometheus.yml`
 `publicIp:9090`

 # Scaling Kubernetes
 `kubectl scale {deployment name} --replicas={desired number of replicas}`