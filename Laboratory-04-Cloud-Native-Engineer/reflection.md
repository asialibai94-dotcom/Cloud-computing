
# Mission Reflection

This laboratory helped me understand the difference between traditional Virtual Machines and containers. When using a Virtual Machine, the system needs to boot an entire operating system before an application can run. This process can take more time and use more RAM and storage because every VM has its own operating system. In comparison, a Docker container shares the host operating system kernel, so it can start much faster and requires fewer resources. During the activity, I was able to pull and run an Nginx container within a short amount of time instead of manually installing an operating system and configuring a web server.

Port mapping is necessary because the web server is running inside the container. The `-p 8080:80` option connects port 8080 on the host machine to port 80 inside the container, where Nginx is listening. This allowed me to access the Nginx server using `curl http://localhost:8080`. Without port mapping, the service inside the container would not be directly accessible through the host's port 8080.

When the `docker rm` command is used, the specified container is removed from the Docker environment. Any data stored only inside that container can be lost when the container is removed, unless the data was stored using a persistent volume or another external storage method.

Containerization also changes how developers and IT operations teams work together. Developers can package applications with their dependencies into containers, while operations teams can deploy the same containers across different environments. This supports DevOps by making deployment more consistent and repeatable.

My GitHub portfolio is also evolving as I add more cloud computing activities and technical documentation. Each laboratory gives me practical experience and creates evidence of the skills I have learned. This activity added Docker, containerization, and cloud-native concepts to my growing portfolio.
