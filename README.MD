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
