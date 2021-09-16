# Web Engineering 2021-2022 / Lab1 Git Race

Please, go to the [Wiki](https://github.com/UNIZAR-30246-WebEngineering/lab1-git-race/wiki) in order to get the instructions for this assignment.

Some ideas for obtaining a :gift: if you are the first that:

- **Moby Dick**: Use Docker to run the app
- **Moby Dick II**: Use Docker Compose to run the app
- **Moby Dick III**: Use Kubernetes (minikube) to run the app
- **Home improvement**: Use a markup template language different from Thymeleaf (server side)
- **Home improvement II**: Use an endpoint that returns the message and update the HTML in client side (no MVC server side)
- **Home improvement III**: Use moder JS framework (React) and a Restful web service (no MVC server side)

User name | NIA | Travis-CI|Score
----------|-----|----------|-----
[UNIZAR-30246-WebEngineering](https://github.com/UNIZAR-30246-WebEngineering/lab1-git-race) |30246 | [![Build Status](https://github.com/UNIZAR-30246-WebEngineering/lab1-git-race/actions/workflows/ci.yml/badge.svg)](https://github.com/UNIZAR-30246-WebEngineering/lab1-git-race/actions/workflows/ci.yml)
Óscar Pueyo Ciutad | 780378 | [![Build Status](https://github.com/iksopo/lab1-git-race/actions/workflows/ci.yml/badge.svg)](https://github.com/iksopo/lab1-git-race/actions/workflows/ci.yml)

# Deployment using docker-compose
In order to run the app, you will need the following packages:
- [docker](https://docs.docker.com/engine/install/)
- [docker-compose](https://docs.docker.com/compose/install)

Run the following command to build the images if needed and run the app:
```
$ docker-compose up
```
It might show the following error:
```
ERROR: Couldn't connect to Docker daemon at [...]
```
Try running with sudo:
```
$ sudo docker-compose up
```
By default, local port 8080 is used to deploy the app, however, it can be modified in ``docker-compose.yml``, setting ``8080:8080`` to ``<your-port>:8080``.