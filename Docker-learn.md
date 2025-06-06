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

Docker uses the client-server architecture. The docker client talks to docker daemon, which does the heavy lifting and building, running, and distributing your Docker containers. The client and daemon run on the same systems. you can connect the docker client to remote docker daemon. Docker client and daemon communicate using REST API, over the UNIX socket or network interface. 

![docker-architecture (1)](https://github.com/user-attachments/assets/e9a87e24-8dbf-45ad-97b6-493737b645e7)

*The Docker daemon*

The Docker daemon (dockerd) listens for the Docker API request and manages docker objects such as images,containers, network, and volumes. A daemon is also communicate with another daemon to manage the Docker services.
*The Docker client*

The Docker client (docker) is the primary way to many Docker user interact with Docker. When you use command like **docker run**, the client sends the commands to **dockerd**, which carried out them. The docker commands uses the Docker API. the Docker client communicate the more than one daemon.

***Docker registries***

A Docker registry stores Docker images. Docker Hub is a public registry that anyone can use, and Docker looks for images on Docker Hub by default. You can even run your own private registry.

When you use the docker pull or docker run commands, Docker pulls the required images from your configured registry. When you use the docker push command, Docker pushes your image to your configured registry.

*Docker objects*
When you are use docker so basically you are creating and usingb images, containers, networks, volumes, plugins, and other objects.

**Images**

A image is a read-only template to create the docker container. a image is based on the another image with some custamization like you build the image which is based on the ubuntu image, but it installs the Apache web server and your application. as well as configuration that neede to run your application.

If you create your own image or you use the image those crete other people and published in the Docker Registry. To build your own image you wright the Dockerfile with the simple step and syntax to create the docker image and run. **so basically each step in the Dockerfile is create the layer in the image. If you change somethings in the dockerfile and rebuild the image that time only those layer are change that you change in the dockerfile are rebuild.** That why the Docker image is Lightweight, small, and fast, when compared to other tools.

**Containers**

A container is running instance of image. You can create, Start, Stop, Delete or Move a container using Docker API or CLI. Also you can connect a container to one or more network, attached storageto it.

By default it is in ois own space on host machine — And its easily talk to each other container or the main system unless you allow it.

You can deside the how "seprate" or "Connected" it is — for things like internet (network), file (storage), and more.

🧳 **Real-World Analogy**

Think of containers as hotel rooms in a big hotel:

🏨 Each room (container) has its own bathroom, bed, and key – it’s private.

🚪 By default, guests in one room can’t enter another — this is isolation.

📞 But the hotel manager (you) can allow shared access — like giving two rooms access to the same Wi-Fi, TV channel, or even a door between them.

In the same way, you can:

Let containers share a network (like same Wi-Fi).

Use the same storage (like shared room fridge).

Or keep them completely private (like no shared access at all).

*A container is defined by its Image as well as configuration you provided when you create and start the image.* 

