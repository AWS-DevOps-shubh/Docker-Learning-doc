# Docker-Learning-doc


*What is Docker?*

Docker is open platform for developing, shipping, and running applications. Docker enable you to seprate your application form infrastructure so you can deliver software quickly.

*Docker Platform*

Docker provides the ability to package and run the application in a loosely isolated enviorment called Docker container(container is a live instance of Image). The isolation and security lets you to run many container simultaneously in given host. Container is light weight and contain everything needed to run the application. So there is no dependancy on host machine to software installed or not on host. Also you can share the container to everyone and docker sure that the conatiner run same in every enviroment and work same.

*What can i use Docker for?*

Fast, consistent delivery of your application
Docker streamline the development lifecycle by allowing the developer to work in standardized enviroment using local containers which provide your application and services. so the container are greatful for CI/CD workflow.

Consider the following example scenario:
![ChatGPT Image Jun 3, 2025, 11_13_32 PM](https://github.com/user-attachments/assets/686a4d71-3963-4f92-8a3a-0e6241ff75ca)


*Responsive deployment and scaling*

Docker container based platform allow you to Highly portable workloads. Doxker container run on local machine, on physical or virtual machine in a data centre or any cloud provider, or in mixture of enviroments.

Doxker portabilty and lightweight nature also give the functionality to make it easy to dynamically manage the wporkload, scaling up or scalling down the applicaton as per the business needed.

*Docker architecture*

Docker uses the client-server architecture. The docker client talks to docker daemon, which does the heavy lifting and building, running, and distributing your Docker containers. The client and daemon run on the same systems. you can connect the docker client to remote docker daemon. Docker client and daemon communicate using REST API, over the UNIX socker or network interface. 

![docker-architecture (1)](https://github.com/user-attachments/assets/e9a87e24-8dbf-45ad-97b6-493737b645e7)


