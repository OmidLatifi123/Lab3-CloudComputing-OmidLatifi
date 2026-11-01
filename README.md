Omid Latifi, Student #1199455

This lab will represent a simple service that might later be deployed to a cloud
platform. No cloud account or paid cloud service is required.

Version control helps a cloud project by tracking every modification to code and infrastructure configurations, enabling safe team collaboration without overwriting work and providing a reliable rollback mechanism if a deployment causes errors.

Assignment #2:

Docker acts like a universal shipping container system for code. Instead of shipping raw code and hoping the target server has the right software versions installed, Docker lets you bundle your code, libraries, and runtime environment together. This makes development, testing, and deployment incredibly fast and consistent

An image is a read-only blueprint or template used to create a container. It is immutable (cannot be changed once built). It contains the application code, core runtime, libraries, environment variables, and configuration files.

A container is a running, executable instance of a Docker image. It is a lightweight, isolated process running on the host machine. Unlike virtual machines, containers share the host operating system's kernel, making them start instantly and use very few resources.

The workflow follows three basic steps: Write a Dockerfiler, Build the Image,Run the Container.


docker build -t cloud-service-demo:1.0 .
docker run -d --name cloud-demo-container -p 8080:80 cloud-service-demo:1.0
