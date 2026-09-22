# Docker Deployment & Lifecycle Documentation

## Lifecycle Commands

1. `docker ps`
   - Lists all actively running containers along with their container IDs, images, ports, and runtime status.

2. `docker stop my-nginx`
   - Gracefully halts the execution of the running `my-nginx` container by sending a `SIGTERM` signal followed by `SIGKILL`.

3. `docker ps -a`
   - Lists all containers on the host, including stopped, paused, and exited containers, verifying that `my-nginx` has stopped.

4. `docker rm my-nginx`
   - Permanently deletes the stopped container instance and its writeable layer from the host system.
