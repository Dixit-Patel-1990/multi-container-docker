
# Frontend Docker Project


[1. For more docker commands and information](https://github.com/Dixit-Patel-1990/Docker)

[2. How to run this project](#Frontend_With_Docker)

[3. Project Architecture](https://drive.google.com/file/d/1OS61RhxUD2yt4cX1PcxGXQ6ljUPnWapI/view)

<!-- [3. Jenkins file to build, test and deploy code to docker hub](https://github.com/Dixit-Patel-1990/Frontend/blob/main/Jenkinsfile) -->

# Frontend_With_Docker

To run react app inside docker container in your local follow following steps,

#### 1. Create an account on https://hub.docker.com/

#### 2. Download Docker desktop and make sure engine is running. We can verify it by running following command on console,
```cmd
docker version
```
This should print something on console.

#### 3. Clone this app by running
```cmd
git clone https://github.com/Dixit-Patel-1990/multi-container-docker.git
```

#### 4. To create container from Dockerfile.dev
```cmd
docker-compose -f docker-compose-dev.yml up --build
```

In the command above we are telling docker, to create containers from docker-compose-dev.yml file.

    1. By default docker build command expects "Dockerfile" that we do not have on PWD so we explicitly need to tell docker by "-f" flag that use "docker-compose-dev.yml" file.

#### 5. Open browser window and type "localhost:3050" you should be able to see the app.


## Authors
- [@Dixit Patel](https://github.com/Dixit-Patel-1990/Docker)
