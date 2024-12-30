# Kuberneties-commands-cheetsheet

The Nautilus DevOps team is planning to deploy some micro services on Kubernetes platform. The team has already set up a Kubernetes cluster and now they want to set up some namespaces, deployments etc. Based on the current requirements, the team has shared some details as below:


Create a namespace named dev and deploy a POD within it. Name the pod dev-nginx-pod and use the nginx image with the latest tag. Ensure to specify the tag as nginx:latest.

Note: The kubectl utility on jump_host is configured to operate with the Kubernetes cluster
--------------------------------
1. At first  kubectl  utility configure and working from jump server, run below commands

    kubectl get namespace

    kubectl get pods
   ---------------------------------------
   2. Create a new namespace as per the task

      kubectl create namespace dev
  --------------------
      To see list of namespaces
      kubectl get namespace

      --------------------------------
      3.  Run the below command to create a pod
kubectl run dev-nginx-pod --image=nginx:latest -n dev



--------------------------------------

 kubectl get pods -n dev



 
      
