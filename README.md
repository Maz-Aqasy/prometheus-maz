# Kubernetes Monitoring using Prometheus

This repository contains Kubernetes YAML configurations for deploying a monitoring stack, including Prometheus and Node Exporter, in a Kubernetes cluster.

## Usage

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/aqasiz/Prometheus-k8s.git
    ```

2. Navigate to the directory containing the YAML files:

    ```bash
    cd Prometheus-k8s
    ```

3. Create NameSpace:

    ```bash
    kubectl create ns monitoring
    ```
  
4. Apply the configurations to your Kubernetes cluster using the `kubectl` command:

    ```bash
    kubectl apply -f <file-name.yaml>
    ```
    
5. Monitor the deployment and check for any issues:

    ```bash
    kubectl get pods -n monitoring
    kubectl logs <pod-name> -n monitoring
    ```
    ``

## Note

- Ensure that you have a running Kubernetes cluster.
- Customize the configurations based on your specific monitoring requirements.
