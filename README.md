# Hello World Flask App

## Build and Run

### Local Development
```bash
pip install -r requirements.txt
python app.py
```

### Docker
```bash
# Build image
docker build -t hello-world:latest .

# Run container
docker run -p 5000:5000 hello-world:latest
```

### Deploy to AWS EKS
```bash
# Install Helm chart
helm install hello-world ./helm-chart

# Get service URL
kubectl get svc hello-world-service
```

## Endpoints
- `/` - Hello World message
- `/health` - Health check