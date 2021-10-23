## Helm

# Instalar

helm upgrade -n wp-demo --create-namespace --install --debug --wait --values=./k8s/values.local.yaml wp-demo ./k8s/helm

# Desinstalar con helm

helm uninstall -n wp-demo wp-demo

## Kubernetes

# Crear todo

kubectl -n wp-demo apply -f .

# Limpiar todo

kubectl -n wp-demo delete -f .

# Ver los Pods

kubectl -n wp-demo get pods

# Ver todo

kubectl -n wp-demo get all
