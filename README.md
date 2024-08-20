# Cloud Native Infrastructure

## Development Environment

### 1. Apply Postgres ConfigMap
```bash
kubectl apply -f cloud-native-postgres-configmap.yaml
```
**Check ConfigMap**
```bash
kubectl get configmap
```

### 2. Apply Postgres Persistent Volume
```bash
kubectl apply -f cloud-native-postgres-pv.yaml
```
**Check Persistent Volume**
```bash
kubectl get pv
```

### 3. Apply Postgres Claim
```bash
kubectl apply -f cloud-native-postgres-pvc.yaml
```
**Check Persistent Volume Claim**
```bash
kubectl get pvc
```

### 4. Apply Postgres Deployment
```bash
kubectl apply -f cloud-native-postgres-deployment.yaml
```
**Check Deployment**
```bash
kubectl get deployment
```

### 5. Apply Postgres Service
```bash
kubectl apply -f cloud-native-postgres-service.yaml
```