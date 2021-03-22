# MockServer with Docker

In this project contains the structure of mocked APIs used in UI automated tests or manual testing when third-party systems are down.

## Technology

This project use the framework [MockServer](https://www.mock-server.com/) used as [Docker](https://hub.docker.com/r/mockserver/mockserver).

## Project structure

The project has the following structure:
  
  ```
      ├──[project_name]
      │  ├──docker-compose.yml
      │  │  
      │  ├──initializerJson.json   
  ```

## Running with Docker
Download and install [Docker](https://www.docker.com/products/docker-desktop).

### Run
Access the project's dir and run:

```sh
$ docker-compose up
```

> **NOTE 1:** Using mock for **Android** must be https.

### Some Docker command line
| Command line | Explanation |
| ------ | ------ |
| docker system prune -a | Clear all dependecies |
| docker ps -a | List all running and stopped containers |
| docker rm ID_CONTAINER | Remove a container |
| docker stop ID_CONTAINER | Stop a container |
| docker imagens | List all imagens |
| docker rmi ID_IMAGE | Remove an imagem |
| docker exec -it ID_CONTAINER bash | Login a container |
| docker-compose up -d | Running unattended|

> **NOTE 1:** Use **docker ps -a** to show the ID_CONTAINER.

> **NOTE 2:** Use **docker images** to show the ID_IMAGE.