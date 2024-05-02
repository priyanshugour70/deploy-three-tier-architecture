# Project Name

In this project i will deploy a three tier architecture.

## Prerequisites

Make sure you have the following installed:

- Kubernetes CLI (kubectl)
- Docker (if you're building Docker images)

## Deployment

1. Clone the repository:
```bash
git clone https://github.com/priyanshugour70/deploy-three-tier-architecture.git
cd deploy-three-tier-architecture
```

2. Apply Kubernetes deployment files:
```bash
kubectl apply -f productcatalogue-service.yaml
kubectl apply -f shopfront-service.yaml
kubectl apply -f stockmanager-service.yaml
```

3. Verify deployments, services, and pods:
```bash
kubectl get deployments
kubectl get services
kubectl get pods
```

4. Access the service:
    - For Product Catalogue:
    ```bash
    kubectl get service/productcatalogue
    ```
    - For Shopfront:
    ```bash
    kubectl get service/shopfront
    ```
    - For Stock Manager:
    ```bash
    kubectl get service/stockmanager
    ```

5. Accessing Services
```bash
Product Catalogue: http://<NodeIP>:<NodePort>
Shopfront: http://<NodeIP>:<NodePort>
Stockmanager: http://<NodeIP>:<NodePort>
```

6. Shutting Down
- To shut down the resources:
```bash
kubectl delete -f productcatalogue-service.yaml
kubectl delete -f shopfront-service.yaml
kubectl delete -f stockmanager-service.yaml
```

## Additional Notes

- The project is based on the [ Java, Spring Boot, git, github, Docker, dockerHub, Docker-compose, Kubernetes, AWS, Terraform, CI/CD and Grafana ] technologies.
- The project is hosted on [GitHub](https://github.com/priyanshugour70/deploy-three-tier-architecture)

## Work
- In the future i will ADD 
- AWS
- Terraform
- CI/CD[Jenkins]
- Grafana