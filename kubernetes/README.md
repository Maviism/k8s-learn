# Learning Kubernetes
# ===========================

## minikube
- Minikube is a tool that makes it easy to run Kubernetes locally.
- Minikube runs a single-node Kubernetes cluster inside a VM on your laptop.
- Minikube is a great way to learn Kubernetes and try out its features without needing a full-blown cluster.
- Minikube is a lightweight Kubernetes implementation that creates a VM on your local machine and deploys a simple cluster inside it.

#### Minikube
[Download here](https://minikube.sigs.k8s.io/docs/start/?arch=%2Fwindows%2Fx86-64%2Fstable%2F.exe+download)

- Install Minikube using the installer or package manager for your operating system.

- Start Minikube with the command `minikube start`.
- This will create a VM and start a single-node Kubernetes cluster inside it.
- You can check the status of your Minikube cluster with the command `minikube status`.
- You can also access the Kubernetes dashboard with the command `minikube dashboard`.

#### Kubectl
- Kubectl is the command-line tool for interacting with Kubernetes clusters.
- Kubectl is used to deploy applications, inspect and manage cluster resources, and view logs.

##### useful commands
- `kubectl get [resource]` - List resources of a specific type (e.g., pods, services, deployments).
- `kubectl describe [resource] [name]` - Show detailed information about a specific resource.
- `kubectl create -f [file]` - Create a resource from a YAML or JSON file.
- `kubectl apply -f [file]` - Apply changes to a resource from a YAML or JSON file.
- `kubectl delete [resource] [name]` - Delete a specific resource.
- `kubectl logs [pod-name]` - View logs for a specific pod.
- `kubectl exec -it [pod-name] -- /bin/bash` - Open a shell in a running pod.


## Kind(service, pod, deployment, etc.)
- A kind is a Kubernetes resource type. Examples include Pod, Service, Deployment, ReplicaSet, StatefulSet, etc.
- Each kind has its own set of properties and behaviors.
- Kinds are defined in YAML or JSON files and are used to create and manage resources in a Kubernetes cluster.
- Kinds are used to define the desired state of a resource in a Kubernetes cluster.
- Kinds are defined in YAML or JSON files and are used to create and manage resources in a Kubernetes cluster.

### Service
- A service is an abstraction that defines a logical set of pods and a policy by which to access them.
- Services enable communication between different parts of an application, such as between a frontend and a backend.
- Services can be exposed to the outside world or kept internal to the cluster.

### Pod
- A pod is the smallest deployable unit in Kubernetes.

### Deployment

### configMap & secret
- ConfigMaps and Secrets are used to store configuration data and sensitive information, respectively.
- ConfigMaps are used to store non-sensitive configuration data, such as environment variables, command-line arguments, and configuration files.

- Secrets are used to store sensitive information, such as passwords, OAuth tokens, and SSH keys.
- Secrets are base64-encoded and can be mounted as files or environment variables in pods.

### StatefulSet
- A StatefulSet is a Kubernetes resource that manages stateful applications.


