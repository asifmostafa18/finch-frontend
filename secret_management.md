Secret Management

Approach
- Using Kubernetes native Secrets
- Secrets are base64 encoded (not encrypted)

Creating Secrets

Create from file
kubectl apply -f kubernetes/secrets/db-secrets.yaml