# ReplicaSet_K8s
ReplicaSet Practices and how to write replicaSet.yaml  and pod.yaml

Firstly we to create pod.yaml file
inside the pod.yaml file we write the code for creation of pod.
how to write yaml file ?
firstly we run the command kubectl explain pod --recursive > pod.txt
this command is create one pod.txt file 
after that with help of the pod.txt file
we write the pod.yaml file with help of pod.txt file
we need to create 4 pods in the k8s cluster so we write 4 times same code and pod name should be different
after that we simple give command in terminal kubectl apply -f pod.yaml
our pods are created
to check the created pods so simple give the command kubectl get pods
-----------------------------------------
follow same process for replicaSet creation
after that give the command kubectl apply -f replicaste.yaml
we see that our rs is created
after that for check our rs run the command kubectl get rs
-----------------------------------------
ImportantNote : Inside metadata labels should be mention in pod.yaml and same labels are write in replicaSet
-----------------------------------------
to check how replicaSet are working?
firstly we are delete one pod, and after that we are check the pod is delete or not.
we saw our pod is deleted and replicaSet is creates new pod replacement of the deleted pod.
------------------------------------------

 kubectl get pods
  11 kubectl run --help
  12 kubectl run akshay --image=nginx
  13 kubectl get pods
  14 kubectl get images
  15 kubectl run --help
  16 kubectl get pods
  17 kubectl get images
  18 kubectl run nginx --image=nginx
  19 kubectl exec --help
  20 kubectl exec akshay bash
  21  kubectl exec akshay -- bash
  22 kubectl exec akshay
  23 kubectl exec --help
  24 kubectl explain --help
  25 kubectl explain pod --recursive > pod.txt
  26 kubectl apply -f pod.yaml
  27 kubectl get pods
  28 kubectl delete pod akshay nginx
  29 kubectl get pods
  30 kubectl --help
  31 kubectl get pods
  32 kubectl delete pod nginx1 nginx2 nginx3 nginx4
  33 kubectl apply -f .\pod.yaml
  34 kubectl get pods
  35 kubectl --help
  36 kubectl label --help
  37 kubectl get pods --show-labels
  38 kubectl get pods --show-labels
  39 kubectl get pods --show-lables
  40 kubectl get pods --show-labels
  41 kubectl describe nginx1
  42 kubectl describe --help
  43 kubectl explain replicaset --recursive > rs.txt
  44 kubectl apply -f .\replicaSet.yaml
  45 kubectl get rs
  46 kubectl get pods
  47 kubectl delete pod akshay-replicaset-25rmj akshay-replicaset-jcwjk akshay-replicaset-q4srj akshay-replicaset-xxrdh
  48 kubectl get pods
  49 kubectl get rs
  50 kubectl delete replicaset akshay-replicaset
  51 kubectl get rs
  52 kubectl apply -f .\replicaSet.yaml
  53 kubectl get rs
  54 kubectl describe pod nginx1
  55 kubectl get pod
  56 kubectl delete pod nginx1
  57 kubectl get pos
  58 kubctl get pods
  59 kubctl get pod
  60 kubectl get pods
  61 kubectl get pods
  62 kubectl describe pod akshay-replicaset-qgct6
  63 kubectl get pods
  64 kubectl delete pod nginx2 nginx3 nginx4
  65 kubectl get pods
  66 kubectl get pods
  67 kubectl describe pod akshay-replicaset-qgct6