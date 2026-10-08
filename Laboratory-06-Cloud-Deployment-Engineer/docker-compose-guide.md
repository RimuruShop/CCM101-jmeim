Docker Compose Guide — Nextcloud + MariaDB
What does the services: block do?
The services: section contains the different containers required for the application. In this setup, it includes the database and app services. Each service has its own image, environment variables, and configuration, allowing Docker Compose to create and manage them together.
How did the Nextcloud app container find the database container?
The Nextcloud app connects to the database through MYSQL_HOST=database. Docker Compose automatically creates a network for the containers and lets them communicate using their service names. Since the database service is named database, the app can use that name to connect without needing the database's IP address.
Difference between docker run and docker-compose up -d
docker run is mainly used to start a single container while specifying its settings through command-line options. In contrast, docker-compose up -d uses the docker-compose.yml file to start multiple services at once, including their configurations, environment variables, and network connections. This makes it easier to manage applications that require several containers.
