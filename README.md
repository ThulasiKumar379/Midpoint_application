# Midpoint_application
Username: administrator

Password: Test5ecr3t

    9  git clone https://github.com/Evolveum/midpoint-kubernetes.git
   10  ll
   11  vi pvc-midpoint-data.yaml
   12  vi pv-midpoint-home.yaml
   13  vi pv-midpoint-data.yaml
   14  kubectl apply -f pvc-midpoint-data.yaml
   15  cat pvc-midpoint-data.yaml
   16  vi pvc-midpoint-data.yaml
   17  kubectl apply -f pvc-midpoint-data.yaml
   18  kubectl create ns midpoint-deployment
   19  kubectl apply -f pvc-midpoint-data.yaml
   20  kubectl create secret generic midpoint-init-pass   --from-literal=passwd=Neoquant@123   -n midpoint-deployment
   21  cd midpoint-kubernetes/deployment/simple
   22  ll
   23  vi 401_statefulset-repository.yaml
   24  kubectl apply -f deployment/simple/
   25  pwd
   26  cd
   27  cd midpoint-kubernetes/
   28  kubectl apply -f deployment/simple/
   29  cd
   30  ll
   31  kubectl apply -f pv-midpoint-data.yaml pv-midpoint-home.yaml
   32  kubectl apply -f pv-midpoint-data.yaml
   33  kubectl apply -f pv-midpoint-home.yaml
   34  kubectl get pods -n midpoint-deployment
   35  kubectl get pvc -n midpoint-deployment
   36  kubectl get pods -n midpoint-deployment
   37  kubectl get pods -A
   38  kubectl get pods -n midpoint-deployment
   39  kubectl delete pod midpoint-0  midpoint-repository-0 -n midpoint-deployment
   40  kubectl get pods -n midpoint-deployment
   41  kubectl logs -f midpoint-repository-0 -n midpoint-kubernetes/
   42  kubectl logs -f midpoint-repository-0 -n midpoint-kubernetes
   43  kubectl gte ns
   44  kubectl get ns
   45  kubectl get pods -n midpoint-deployment
   46  kubectl describe pod midpoint-repository-0 -n midpoint-deployment
   47  mkdir -p /mnt/data/midpoint-repository
   48  kubectl get pods -n midpoint-deployment
   49  kubectl get svc -n midpoint-deployment
   50  kubectl patch svc midpoint -n midpoint-deployment   -p '{"spec": {"type": "NodePort", "ports": [{"port": 8080, "targetPort": 8080, "nodePort": 30080}]}}'
   51  kubectl get svc -n midpoint-deployment
   52  curl -kv 18.191.186.182:30080/midpoint
   53  kubectl get pod midpoint-0 -n midpoint-deployment -o wide
   54  kubectl get pods -n midpoint-deployment
   55  kubectl describe pod midpoint-0 -n midpoint-deployment
   56  kubectl get pods -n midpoint-deployment
   57  kubectl logs -f midpoint-0 -n midpoint-kubernetes
   58  kubectl logs -f midpoint-0 -n midpoint-deployment
   59  kubectl get pods -n midpoint-deployment
   60  kubectl logs -f midpoint-0 -n midpoint-deployment
   61  kubectl get svc -n midpoint-deployment
   62  kubectl delete svc midpoint -n midpoint-deployment
   63  cd midpoint-kubernetes/
   64  kubectl apply -f deployment/simple/
   65  kubectl get pods -n midpoint-deployment
   66  kubectl delete pod midpoint-repository-0 -n midpoint-deployment
   67  kubectl delete pod midpoint-0 -n midpoint-deployment
   68  kubectl get pods -n midpoint-deployment
   69  kubectl logs -f midpoint-0 -n midpoint-deployment
   70  kubectl get pods -n midpoint-deployment
   71  kubectl get svc -n midpoint-deployment
   72  kubectl get pods -n midpoint-deployment
   73  kubectl get svc -n midpoint-deployment
   74  kubectl get pods -n midpoint-deployment
   75  kubectl get svc -n midpoint-deployment
   76  curl http://10.99.42.69:8080/midpoint
   77  curl -kv http://10.99.42.69:8080/midpoint
   78  kubectl edit svc midpoint -n midpoint-deployment
   79  kubectl get pods -n midpoint-deployment
   80  kubectl get svc -n midpoint-deployment
   81  kubectl get pods -n midpoint-deployment
   82  curl -kv http://18.191.186.182:30967/midpoint
   83  kubectl get pods -n midpoint-deployment
   84  kubectl exec -it midpoint-0 -n midpoint-deployment -- env | grep -i midpoint
   85  history
[root@ip-172-31-2-247 midpoint-kubernetes]#
