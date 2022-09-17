# Deploy a Kubernetes cluster in one minute is possible, is it?
Simple Kubernetes Deployments and Configurations

## Configurations

Configuration is key because it might break your whole app if you do not set it up correctly. You can follow along with these configs but do not forget that your computer and mine are not the same. Operating systems, dependencies, software, VMs, versions are somewhat different.

### Kubernetes setup

Minikube was chosen to be the playground for this project. It is simple and has a good documentation. 

There are other available options: k3s, Kind, Kubeadm, Rancher.

`brew install minikube`

then install the kubectl CLI because it reduces the amount of characters/commands you'll type.

`brew install kubectl`

To start Minikube with a specific driver.

`minikube start --driver=hyperkit`

To verify if it is correctly configured.

`minikube status`

### DockerHub images

You can choose images and its tags you want and it should be a good fit for your project.

### MongoDB setup

The connection string is supposed to be secret and specific to a user.

For example:
```
mongodb+srv://<u>:<p>@<project>.2cspo.mongodb.net/<c>?retryWrites=true&w=majority
```

You have to change values in angle brackets according to your info.

- `<u>` is your username
- `<p>` is your password
- `<project>` is your desired project
- `<c>` is your collection in a project

> There are several methods you can use to connect to MongoDB.

1. Via the MongoDB Shell.
2. Directy in your application.
3. Via the MongoDB Compass.
4. Using VS Code.

### Web/App setup

You can use any website or app to try and see if there's a bug. I use my side project that I built a while ago with NextJS. It seems to work really well. 
