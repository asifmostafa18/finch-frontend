Kubernetes Architecture

Components
Frontend
   - Deployment with 2 replicas
   - Exposed via LoadBalancer service on port 80

Backend
   - Deployment with 2 replicas
   - ClusterIP service on port 3000

PostgreSQL
   - Single replica deployment
   - Persistent storage via PVC
   - ClusterIP service on port 5432

Redis
   - Single replica deployment
   - Persistent storage via PVC
   - ClusterIP service on port 6379


kubectl apply -f kubernetes/