### SRE Assignment
#### Simple counter application written in Python using flask and deployed on Kubernetes(minikube)

#### Prerequisites
1. VS Code/Pycharm - Text editor/IDE.
2. Docker Desktop.
3. Kubernetes CLI.
4. Minikube.
5. Python 3.8
   
How to Deploy on kubernetes?
1. Start with cloning git repo to local machine 
`git clone https://github.com/RohithSB/counter-web-application.git`
2. Navigate to `counter-web-application` folder.
3. Startup the Docker desktop, then execute the command below
   `docker build --tag counter-app:latest .`
4. Once docker build is succesfull and image is built, now we can deploy to kubernetes engine.
   `kubectl apply -f deployment.yaml`
5. Access the application using the command below
   `minikube start service: counter-service`
6. Do port forward using below cmd.
   `kubectl port-forward service/counter-service portno:6000`
