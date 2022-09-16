# Deploy a Kubernetes cluster in one minute is possible, is it?
Simple Kubernetes Deployments and Configurations

## Configurations

### Kubernetes setup

Minikube was chosen to be the playground for this project. It is simple and has a good documentation. 

There are other available options: k3s, Kind, Kubeadm, Rancher.

`brew install minikube`

then install the kubectl CLI because it reduces the amount of characters/commands you'll type.

`brew install kubectl`

### DockerHub images

You can choose images and its tags you want and it should be a good fit for your project.

### MongoDB setup

The connection string is supposed to be secret and specific to a user.

`mongodb+srv://<username>:<password>@<projectname>.2cspo.mongodb.net/<collectionname>?retryWrites=true&w=majority`

> There are several methods you can use to connect to MongoDB.

1. Via the MongoDB Shell.
2. Directy in your application.
3. Via the MongoDB Compass.
4. Using VS Code.

### Web/App setup
