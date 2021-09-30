# docker-aula-devops

docker build -t gcr.io/${PROJECT_ID}/myfirstapp:2.0 .
		  
docker push gcr.io/${PROJECT_ID}/myfirstapp:2.0

kubectl apply -f myfirstapp-service.yaml -n labgke

kubectl apply -n labgke -f myfirstapp-deployment.yaml

kubectl get deployment -n labgke

kubectl describe deployment myfirstapp -n labgke

kubectl get pods -n labgke
