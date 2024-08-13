
# Criar imagem

Instruções de como criar imagem do docker e disponibilizar no Docker Hub


## Gerar docker file


```bash
  docker build -t meu-servidor-tomcat-mysql .

```



## Executar o contêiner Docker
```bash
  docker run -d -p 8080:8080 -p 3306:3306 meu-servidor-tomcat-mysql

```
    

## Subir no Docker Hub

Etapas:

```bash
  docker login

```
```bash
  docker tag meu-servidor-tomcat-mysql seu-usuario/meu-servidor-tomcat-mysql

```
```bash
  docker push seu-usuario/meu-servidor-tomcat-mysql

```

## Baixar e rodar do repositório original

```bash
  docker pull kopecode/meu-servidor-tomcat-mysql

```
```bash
  docker run -d -p 8080:8080 -p 3306:3306 kopecode/meu-servidor-tomcat-mysql

```

## Repositório Docker

 - [Docker](https://hub.docker.com/r/kopecode/meu-servidor-tomcat-mysql)
