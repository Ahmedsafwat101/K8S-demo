# K8S-demo

This is a simple demo using the most popular Kubernetes components
  

## Components 

- ConfigMap

- Secret

- Deployment

- Service external & internal 

## Details 

- ConfigMap
           
        A ConfigMap is an API object used to store non-confidential data in key-value pairs, can be consumed as a as environment variables in pods.

- Secret
           
      A Secret is an object that contains a small amount of confidential data such as a password, a token, or a key. Such information might otherwise be put in a Pod specification or in a container image.

- Deployment
           
      A Deployment provides declarative updates for Pods and ReplicaSets.

      You describe a desired state in a Deployment, and the Deployment Controller changes the actual state to the desired state at a controlled rate. You can define Deployments to create new ReplicaSets,
      or to remove existing Deployments and adopt all their resources with new Deployments.      

- Service

      An abstract way to expose an application running on a set of Pods as a network service.




## Run Locally

Clone the project

```bash
  git clone https://link-to-project
```

Go to the project directory

```bash
  cd my-project
```

Create the Deployment  

```bash
  kubectl apply -f .\mongo-config.yaml 
  kubectl apply -f .\mongo-secret.yaml 
  kubectl apply -f .\mongo.yaml 
  kubectl apply -f .\webapp.yaml 
```

Get Node details 

```bash
  kubectl get all -o wide
```





![App Screenshot](https://github.com/Ahmedsafwat101/K8S-demo/blob/master/screenshots/getalldetails.png)

