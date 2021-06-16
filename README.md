# k8smongodbstateful


this repository is for creating mongodb instances using helm in ubantu 

first execute 

kubectl apply -f pv.yml 
helm install mongo -f mongovalues.yml  bitnami/mongodb


hola !! 

go 
kubectl get pods 
kubectl get pv, pvc 

for persistance volume and persistance volume claim 

helm is like package manager for kubenates (All the configuration handled by bitnami/mongodb) 

nohup kubectl port-forward --namespace default svc/mongo-mongodb 27017:27017 

now test with 

kubectl exec -it mongo-mongodb-0 -- mongo
mongo --host 127.0.0.1 --authenticationDatabase admin -p $MONGODB_ROOT_PASSWORD






