# istio-traffic-mgmt
Ejemplos para manejar el tráfico con istio service mesh

Requisitos de software: 

- Tener acceso a un cluster de kubernetes de preferencia con versión v1.20.2 o superior.Para instalar localmente podemos usar Minikube, Docker Desktop, Rancher, MicroK8s, entre otros
- Tener instalado Kubernetes CLI (guía: https://kubernetes.io/docs/tasks/tools/)
- Tener instalado Istio CLI para realizar la instalación de Istio versión 1.21.0 (guía: https://istio.io/latest/docs/setup/getting-started)

Requisitos de hardware:
- mínimo 16 GB de RAM y 4 CPUs


Instalación:
>> istioctl install --set profile=demo
✔ Istio core installed                                                          
✔ Istiod installed                                                              
✔ Egress gateways installed                                                     
✔ Ingress gateways installed                                                    
✔ Installation complete  

>> kubectl label namespace default istio-injection=enabled
