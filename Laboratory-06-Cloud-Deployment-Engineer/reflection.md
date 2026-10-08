# Reflection

Creating a `docker-compose.yml` file makes the work of a cloud engineer much easier because the whole application setup, including containers, environment variables, ports, and dependencies, can be organized in one file. Instead of entering multiple `docker run` commands, a single command can be used to start the entire application. The file can also be used as documentation, saved in version control, shared with others, and reused in different environments.

YAML requires proper indentation, so even a small formatting mistake, such as using a Tab instead of spaces, can cause the configuration to fail. When this happens, Docker Compose may show a syntax error and prevent the containers from starting. This showed me the importance of maintaining consistent spacing when creating or editing Compose files.

We used environment variables such as `MYSQL_PASSWORD` to keep important configuration details separate from the main application settings. This makes the credentials easier to manage and allows the same Docker image to work in different environments by changing the variables. Using an external `.env` file can also help prevent sensitive information from being stored directly in version control.

Being able to deploy a working cloud storage system within a few minutes gave me a better understanding of what cloud engineers do. Instead of manually setting up every component, Docker Compose handled most of the infrastructure setup. It showed me how Infrastructure as Code can simplify complicated deployment processes.

Since Mission 1, my view of cloud computing has changed. I previously thought of the cloud mainly as "someone else's computer," but I now understand that cloud computing also involves creating infrastructure that can be automated, repeated, and managed efficiently. From setting up a virtual machine and managing storage to connecting multiple containers, I have learned how infrastructure can be controlled through code instead of being configured manually.
