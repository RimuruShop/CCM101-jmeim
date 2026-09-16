# Mission 4 Reflection

In this activity, I learned that deploying applications using Docker can be much faster and simpler than using a Virtual Machine. A VM requires an entire operating system, virtual hardware, and additional resources before an application can run. Docker containers, on the other hand, use the host system's kernel and can start an application in just a few seconds.

I also learned the importance of port mapping, such as `-p 8080:80`. The Nginx web server runs on port 80 inside the container, but the container's network is separated from the host. By mapping port 8080 on the host to port 80 inside the container, I was able to access the Nginx server through `localhost:8080`.

Another important lesson was understanding what happens when a container is removed using `docker rm`. Files and data stored directly inside the container can be lost when the container is deleted. For data that needs to remain available, Docker volumes or bind mounts should be used because they store data outside the container itself.

This activity also helped me understand how containerization makes application deployment more consistent. Since Docker containers include the application and its required dependencies, the same container can be used across development, testing, and production environments. This helps reduce compatibility problems and makes the deployment process easier.

Overall, this mission added another useful skill to my GitHub portfolio. Through this activity, I gained practical experience with Docker, containers, port mapping, and container management. It also helped me better understand how containerization is used in modern cloud and DevOps environments.
