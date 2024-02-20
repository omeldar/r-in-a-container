# Programming with R in a container

This setup allows you to work with R in R Studio in the browser.

## Setup

You will have to install Docker first if you haven't already.

1. Clone repository with

HTTPS:
```
git clone https://github.com/omeldar/r-in-a-container.git
```
SSH:
```
git@github.com:omeldar/r-in-a-container.git
```

2. Execute the command below in the git repositories folder. This step might take 2-5 minutes depending on your device's performance.

```
docker compose up -d
```

3. When the container has started go to your browser and visit: [http://localhost:8787/](http://localhost:8787/)
4. Log in with user: **rstudio** and default password: **Init1234**

## Installing R packages

Install additional r packages using the below command directly in RStudio

```
install.packages("package-name")
```

_Replace 'package-name' with the package you want to install._

## Changing user and password

If you want to change the username and password to log in, you can do so in the `docker-compose.yml` under `environment`.
