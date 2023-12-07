# Example of initial configuration of a Sonarqube server with docker

## Technologies
- Sonarqube 9.9.3-community
- Postgres 16.1

## Environment preparation
- You must have Docker and Docker Compose installed.
- To correctly create the docker volumes defined in the 'docker-compose.yml' file, the folders must be created as described below.
```
example-sonarqube
|   docker-compose.yml
|   README.md
|   .gitignore   
|__ postgresql
|   |__ data
|
|__ sonarqube
    |__ data
    |__ extensions
    |__ logs
    |__ temp
```

## To execute
- Open the terminal inside the example-sonarqube folder and run the command below.
``` bash
docker compose up --build
```
- Open the url 'http://localhost:9000' in the browser and you will have access to Sonarqube.
