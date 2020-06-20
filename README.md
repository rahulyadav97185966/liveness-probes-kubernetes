# liveness-probes-kubernetes
  this repository contains an example explanation of the use of probes specially liveness probes. <br>
  Official Doc : https://kubernetes.io/docs/tasks/configure-pod-container/configure-liveness-readiness-startup-probes/

# what is Probes in kubernetes and Why we use it in production level Scenario.
     As Probes name suggest the probes is used for testing and checking the health of any circuit in electronics using that ammeter or other. similarly in kubernetes we use probes for the health check and testing of application (pods) . for Example, We developed one application and run it application is prefectly coded and it does not have any errors but when user is using it he is unable to access that application in these case we have to reboot the application of we have to find the errors in the application. (like when our laptop gets stuck we do reboot.
     
     
# Commands That Checks the Application Health :

     $ cat > liveness.yml : copy the code given in the liveness.yml file and paste it. it contains all the instrcution taht checks health and if that application is unhealthy it deletes that file and again restarting and again creating the file.  
     $ vi pr.yml  : You can see the  code using this command.
     $ kubectl create -f liveness.yml : it is creating a pod.
     $ kubectl get pods -w : You can see the pods are running or not using this commnad
     $ kubectl get nodes : you can see the nodes.
     $ kubectl describe pod liveness-exec : Using these command you can see the status of the application(pod).
   


