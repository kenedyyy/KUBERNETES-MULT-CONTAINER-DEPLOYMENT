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



