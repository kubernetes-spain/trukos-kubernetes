# ¿Qué es Kubernetes? - Kubernetes
Kubernetes es un sistema de código libre para la automatización del despliegue, ajuste de escala y manejo de aplicaciones en contenedores​ que fue originalmente diseñado por Google y donado a la Cloud Native Computing Foundation. Soporta diferentes entornos para la ejecución de contenedores, incluido Docker

# Controladores
Deciden donde levantar los contenedores con sus variable de entornos.

# Workers
Donde van a correr esos contenedores, son descartables.

# Servidores etcd
Donde se guardan los datos

# namespaces
sub-cluster, ejemplo para crear dentro de un mismo cluster dos entornos

# pods
Conjunto de contenedores.

# Copiamos el archiov de conexion yaml
```
mv k8s-1-17-5-do-0-sfo2-1589321851845-kubeconfig.yaml /home/marlon/.kube/config
```

# Ver los workers
```
kubectl get nodes
kubectl get nodes -o wide
```

# nano 00-namespace.yaml
# kubectl apply -f 00-namespace.yaml
```
kind: Namespace
apiVersion: v1
metadata:
  name:testing
```
```
kubectl get ns
```


