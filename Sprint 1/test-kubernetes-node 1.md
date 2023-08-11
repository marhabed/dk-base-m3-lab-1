# Probar Kubernetes en nodo 1

Objetivos
- Crear namespace y pods monitoreando su estado con la modalidad watch

Tareas
Crear namespace, monitorear cambios a etiquetas en modalidad watch
Monitorear cambios a eventos de pods, crear pod de corta duración

-------------------
$ kubectl get namespace hello-hc -o yaml  
apiVersion: v1  
kind: Namespace  
metadata:  
  creationTimestamp: "2023-08-11T02:40:40Z"  
  labels:  
    kubernetes.io/metadata.name: hello-hc  
  name: hello-hc  
  resourceVersion: "3698"  
  uid: c47bf82c-8aa9-47b5-8ff6-843fe289769a  
spec:  
  finalizers:  
  - kubernetes  
status:  
  phase: Active  

