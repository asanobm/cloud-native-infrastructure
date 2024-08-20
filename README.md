# Cloud Native Infrastructure

## Development Environment

### 1. Apply Postgres ConfigMap
```bash
minikube minikube kubectl -- apply -f cloud-native-postgres-configmap.yaml
```
**Check ConfigMap**
```bash
minikube kubectl -- get configmap
```

### 2. Apply Postgres Persistent Volume
```bash
minikube kubectl -- apply -f cloud-native-postgres-pv.yaml
```
**Check Persistent Volume**
```bash
minikube kubectl -- get pv
```

### 3. Apply Postgres Claim
```bash
minikube kubectl -- apply -f cloud-native-postgres-pvc.yaml
```
**Check Persistent Volume Claim**
```bash
minikube kubectl -- get pvc
```

### 4. Apply Postgres Deployment
```bash
minikube kubectl -- apply -f cloud-native-postgres-deployment.yaml
```
**Check Deployment**
```bash
minikube kubectl -- get deployment
```

### 5. Apply Postgres Service
```bash
minikube kubectl -- apply -f cloud-native-postgres-service.yaml
```

### 6. Port forward
```bash
minikube kubectl -- port-forward service/postgres 15432:5432
```