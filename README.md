# KUBERNETES-MULTI-CONTAINER-DEPLOYMENT

+ Container applications are essentialy software that can virtually package and isolate applications for deployment,splitting this further into multiple containers helps you to bettre isolate and maintain key services tha will then make it more beneficial in running more complex and intensive applications.

+ The purpose of this video will be to give a step by step tutorial on how to deploy your multicontainer application using the kubernetes ochestration system in docker. an overview and explanation on kubernetes can be found [here](https://kubernetes.io/)

+ ### Table of contents 
+ [Client configuration and its service]( #client-configuration-and-its-service )
+ [Postgress,its service  and persistent volume claim configuration]
+ [server configuration and its service]
+ [Ingress Nginx controller installation and configuration]
+ [Run deployed application on kubernetes]
+ [Undeploy application from kubernetes]

+ ### Prerequisites 
+ A comprehensive understanding of container technology and [docker](https://www.docker.com/resources/what-container), [Node Js](https://www.w3schools.com/nodejs/nodejs_intro.asp), [ingress](https://kubernetes.io/docs/concepts/services-networking/ingress/),  [Nginx](https://www.nginx.com/resources/glossary/nginx/), [postgess](https://www.postgresql.org/) and [react](https://reactjs.org/tutorial/tutorial.html).
+ [Docker](https://docs.docker.com/docker-for-windows/install/) installed in your working environment and enable [kubernetess](https://birthday.play-with-docker.com/kubernetes-docker-desktop/)
+ [Install postgress as a database server](https://www.postgresql.org/download/)
+ Make sure your code editor has instaaled the extensions ffor the above mentioned sofware(I would recommend [visual studio](#https://visualstudio.microsoft.com/)

## client configuration and its service
+ we wil begin by creating a new folder which we will label k8s
+ within the folder we will create a client deployment .yml file which we will use to define our client 
+ we will begin by defining our client
![Screenshot 2021-11-15 114818](https://user-images.githubusercontent.com/79918151/144392049-05e988c6-126c-4a69-ab42-1b931d1b6a24.png)
after defining our client we will move fowward to the metadata section
here we will define our component replicas selector matchlabels and selectror
we will then move to the spec section where we will define the image we ill be using during the deployment
after defining we will move to the terminal where we will test the file by using the command kubectl apply -f with the name of he folder we will created as so
note that we can apply a complex folder wih this command under k8s for every file that will be preceded

we will begin by creating a service configuration file in which we will label  as client cluster service ip service .yml 
we will begin by defining the service 
we will then move to  the specifications and ports 
and then test the file and apply the pods to the terminal

we will create a new file for tthe server by first beginning by creating a postgres deployment. yml
we will first define the file  
then we will mve to define the spec 
we will then efine he template

we will create a persistence volume claim folder for the postgresand define it
in the specification area  we will define our accwss mode whih we will set as readwriteonce
we will hen assign the storage for testin purposes
we will continue writing the settings of the postgres deployment
we will define the volume
we will then move back to the postgres file where we will define the containers
we will then define the ports in which we will use the default port 5432
we will then add a volume mount section to link the previously defined volume and this section
we will ithen add an environment setion to define the environment variables 
we will then create the password 






