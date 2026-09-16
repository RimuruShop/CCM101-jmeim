
# Docker Deployment Log

| Command                | What It Does                                                    | Result                                                                         |
| ---------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------ |
| `docker ps`            | Lists all currently running containers.                         | Confirmed that the `my-nginx` container was running and mapped to port `8080`. |
| `docker stop my-nginx` | Gracefully stops the running `my-nginx` container.              | The container was successfully stopped.                                        |
| `docker ps -a`         | Lists all containers, including running and stopped containers. | Confirmed that `my-nginx` was stopped with status **Exited (0)**.              |
| `docker rm my-nginx`   | Permanently removes the stopped container from the host.        | The `my-nginx` container was successfully removed.                             |

### Terminal Output

```text
CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS         PORTS                                     NAMES
52152761da98   nginx     "/docker-entrypoint.…"   2 minutes ago   Up 2 minutes   0.0.0.0:8080->80/tcp, [::]:8080->80/tcp   my-nginx

my-nginx

CONTAINER ID   IMAGE     COMMAND                  CREATED         STATUS                              PORTS     NAMES
52152761da98   nginx     "/docker-entrypoint.…"   2 minutes ago   Exited (0) Less than a second ago             my-nginx

my-nginx
```

### Short Explanation

The commands were used to verify and clean up the Nginx Docker container. First, `docker ps` confirmed that `my-nginx` was running on port `8080`. The container was then stopped using `docker stop my-nginx`. After checking with `docker ps -a`, the container showed an **Exited (0)** status, confirming that it stopped successfully. Finally, `docker rm my-nginx` removed the container from the system.
