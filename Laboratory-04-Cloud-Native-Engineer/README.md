# Laboratory Activity 4: The Cloud-Native Engineer

## Mission Overview
This laboratory explores containerization fundamentals, contrasting traditional virtualization with container architectures. Using the KillerCoda interactive cloud terminal, an Nginx web server was pulled, deployed via port forwarding, verified through HTTP requests, and managed throughout its operational lifecycle.

## Objectives
- Differentiate between traditional Virtual Machines (VMs) and Containers.
- Access and inspect a Docker-enabled Linux environment in KillerCoda.
- Pull, configure, expose, and deploy containerized services via the Docker CLI.
- Manage container states: listing, stopping, and removing containers.
- Structure technical documentation and evidence in a version-controlled repository.

## Docker Commands Executed
- `docker --version`: Displays the installed Docker client and engine versions.
- `docker info`: Outputs system-wide Docker configuration, running container counts, and storage drivers.
- `docker pull nginx`: Fetches the official Nginx container image from Docker Hub.
- `docker run -d -p 8080:80 --name my-nginx nginx`: Runs the Nginx image as an isolated detached process mapping host port 8080 to container port 80.
- `curl http://localhost:8080`: Sends an HTTP GET request to verify the server responds with the default Nginx welcome page.
- `docker ps`: Lists active, running containers.
- `docker stop my-nginx`: Stops the running container instance gracefully.
- `docker ps -a`: Lists all containers (active and terminated) on the system.
- `docker rm my-nginx`: Removes the stopped container instance permanently.

## Skills Learned
- Docker CLI container orchestration and flag syntax (`-d`, `-p`, `--name`).
- Port redirection principles between host network interfaces and isolated container namespaces.
- Diagnosing container runtime states and reading lifecycle process outputs.
- Technical Markdown documentation for cloud operations.

## Challenges Encountered
- **Port Mapping Verification**: Ensuring the host port (`8080`) was distinct from the internal container port (`80`) to prevent port conflicts with standard system services.
- **Detached Execution**: Remembering to execute web servers using `-d` so the interactive terminal prompt was not held hostage by foreground container logs.
