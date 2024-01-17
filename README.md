Prequisite
- Enable metrics-server in minikube with this syntax:
minikube addons enable metrics-server

ToDo
- Build vpa component in autoscaler folder:
./autoscaler/vertical-pod-autoscaler/hack/vpa-up.sh

- Create all components (Deployment, Service, and VPA):
kubectl create -f .

- To get accessible address, run:
minikube service list

- Syntax to test app:
ADDRESS:PORT/jktt <--Diplay Jakarta time
ADDRESS:PORT/spt <--Diplay Sothpole time
ADDRESS:PORT/nyct <--Diplay Newyork time

- Clean everything with :
kubectl delete -f .
./autoscaler/vertical-pod-autoscaler/hack/vpa-down.sh
