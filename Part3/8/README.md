I created a kubernetes cluster to digital oceans platform and i had to install the
kubernetes management client kubectl.

Digitalocean provided a ready-made config for the kubectl and then i just had to follow a few tutorials to figure out the deployment.yml and service.yml files and deploy the application.  
For this i used the same golang react app that i had used for the earlier task.  
The app is running behind load balancer and is utilizing two nodes, which i assume are two separate hosts like mentioned in the exercise.

The deployment was really simple after all the config had been done, just execute the commands 

````
kubectl apply -f deployment.yml
kubectl apply -f service.yml
````

and the app was running in http://167.99.17.173/