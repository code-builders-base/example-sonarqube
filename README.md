# Exemplo de configuração inicial de um servidor Sonarqube com docker

## Tecnologias
- Sonarqube 9.9.3-community
- Postgres 16.1

## Preparação do ambiente
- É necessário ter o Docker e o Docker Compose instalados.
- Para criação correta dos volumes do docker definidos no arquivo 'docker-compose.yml' é necessário que sejam criadas as pastas conforme descrito abaixo.
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

## Para executar
- Abrir o terminal dentro da pasta example-sonarqube e executar o comando abaixo.
``` bash
docker compose up --build
```
- Abrir a url 'http://localhost:9000' no navegador e terá acesso ao Sonarqube.
