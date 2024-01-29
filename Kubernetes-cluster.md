# Kubernetes
## Creating a cluster using KinD
Note: Docker should be installed
### Install Kind on Linux - 
  1. Use the curl command to download Kind. 
  
    curl -Lo ./kind https://kind.sigs.k8s.io/dl/v0.14.0/kind-linux-amd64
    
   2. Change the binary's permissions to make it executable.
   
    chmod +x ./kind
    
   3. Move kind to an application directory, such as /bin.
   
    sudo mv ./kind /bin/kind
    
### Using Kind to Create a Development Environment -
  1. To create a cluster with a different name, use the --name option.
  
         kind create cluster --name=[cluster-name]
      
  2. Confirm the cluster deployment with kubectl.
  
         kubectl get nodes
      
  *note*: if returns, ""kubectl" command not found" then install kubectl using snap.
   
      snap install kubectl --classic
      
   3. Check the Created Cluster with get.
   
          kind get clusters
      
   4. To Delete the Cluster.
    
          kind delete cluster
    
    
   
    
