# Exemplo de configuração inicial de um servidor Sonarqube com docker

* Para criação correta dos volumes do docker definidos no arquivo 'docker-compose.yml' é necessário que sejam criadas as pastas conforme descrito abaixo.
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