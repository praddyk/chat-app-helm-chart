# chat-app-helm-chart
This project is regarding the deployment of a chat app similar to the whatsapp. 
 we will take the frontend and backend app build image, push to registry, build the manifest files, deploy it to the k8s.
what all to install (all have to run local)

- docker
- helm
- minikube/kind/

features of the project:-
1. the end to end deployment project 
1. Decoupling the developer and infra enginner's deployments.
2. using helm template to generate the required env manifest file.
3. has multi container pods with nginx, app, filebeat.
4. has node affinity and taint & tolerance on the pods and namespace.

This project tools:-
- image build :- docker
- image registry :- docker hub
- CICD tool - github-actions
- Environment:- dev, qa, prod
- infra provisioning :- terraform
- package manager:- helm chart
- depolyment :- EKS(prod),minikube(dev)
- programming lang :- yaml,HCL,Golang
- middleware 
    - node -> current-alpine3.19
    - nginx -> 1.25.1

High level deployment architecture
![High level deployment architecture](/images/high-level-deployment-process.png)

Pod-architetcture
![Pod-architetcture](/images/pod-architecture.png)
