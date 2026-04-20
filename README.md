# kubernetes_practice

create shortcut for commands
$ sudo vim /etc/profile
$ alias k='kubectl'            
$ sudo source /etc/profile
      
- create a pod 
$ kubectl apply -f <pod.yml>
$ sudo kubectl get pod
$ sudo kubectl get pod -o wide
$ sudo kubectl get service
$ sudo kubectl get service -o wide
$ sudo kubectl describe pod
$ sudo kubectl exec -it <podname> -- /bin/bash
$ sudo kubectl get endpoints
$ sudo kubectl delete pod <pod_name>
$ sudo kubectl delete pod --all
$ sudo kubectl delete service <service_name>
$ sudo kubectl delete service --all
$ sudo kubectl logs <pod_name>
$ sudo kubectl get pod <pod_name> -o yaml
$ sudo kubectl get pod <pod_name> -o json
$ sudo kubectl scale pod replica = 10
$ sudo kubectl get rc
$ sudo kubectl scale rc myrc --replicas=6 &&  kubectl get rc mrc --watch
