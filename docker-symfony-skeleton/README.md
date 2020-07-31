## Description
Modern, developer friendly LEMP stack with Symfony Framework and some useful tools. 

Includes: 
- `nginx:alpine`,
- `mariadb`,
- `php:fpm-alpine`,
- `symfony 5.0.*`,
- `phpmyadmin`,
- `git`,
- `composer`


---

## How to use
### Launching
```
git clone https://github.com/e-sence/docker.git ./
cd docker-symfony-skeleton/docker
docker-compose -p symfony up
```

---

### Shutdown
Stops containers and removes containers, networks, volumes, and images created by `up`.
- `docker-compose -p symfony down`

---

### Container information
Display detailed information on network
- `docker network inspect symfony_default`

---

### Prune containers
When you stop a container, it is not automatically removed unless you started it with the `--rm` flag. To see all containers on the Docker host, including stopped containers, use `docker ps -a`. You may be surprised how many containers exist, especially on a development system! A stopped container’s writable layers still take up disk space. To clean this up, you can use the docker container prune command.
- `docker builder prune`

---

### Links
- Symfony app: `http://localhost/`
- Phpmyadmin: `http://localhost:8000/`