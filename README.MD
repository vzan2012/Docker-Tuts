# Docker - Tutorials

The below commands are for the reference and that I have learnt from the course authored by Stephen Grider.

---

## Commands

- Check the docker version

  ```console
    docker version
  ```

- Creating and Running a Container from an Image

  `docker run <image_name>`

  _Example:_

  ```console
    docker run hello-world
  ```

- Running Busybox

  ```console
    docker run busybox echo Welcome
  ```

  ```console
    docker run busybox ls
  ```

- List all running containers

  ```console
    docker ps
  ```

- List all running containers ever created

  ```console
    docker ps --all
  ```

- `docker run`

  **docker run = docker create + docker start**

- Start or Restart a ccontainer

  ```console
    docker start -a <<container_id>>
  ```

- To remove all container in the system

  ```console
  docker system prune
  ```

- Get logs from a container

  ```console
  docker logs <<container_id>>
  ```

- Stop a container

  ```console
  docker stop <<container_id>>
  ```

- Kill a container
  ```console
  docker kill <<container_id>>
  ```
- To remove all container in the system
  ```console
  docker system prune
  ```

**Example:**

```console
docker run redis
```

- Execute an additional command in a container

  ```console
  docker run -it <<container_id>> <<command>>
  ```

- To run a shell command inside of container

  ```console

  docker run -it <<container_id>> sh

  ```

  ```console
  docker run busybox sh
  ```

- Build a docker image

  ```console
  docker build .
  ```

- Build a docker image with the tag name

  ```console
  docker build -t <<docker_username>>/<<image_name>> .
  ```

- Run or Execute the Docker container

  ```console
  docker run -p <<mymachine_port_number>>:<<container_port_number>> <<image_name>>
  ```

- For multiple local containers use the _docker-compose_

  _docker run <<image_name>>_ equivalent to

  ```console
  docker-compose up
  ```

  ```console
  docker build .
  docker run <<image_name>>

  docker-compose up --build
  ```

- Stop multiple containers running
  ```console
  docker-compose down
  ```

Docker restart policies are **_no_, _always_, _on-failure_, _unless-stopped_**.

- Docker Compose - container status
  ```console
  docker-compose ps
  ```
