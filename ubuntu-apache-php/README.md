
# Criar imagem

Instruções de como criar imagem do docker e disponibilizar no Docker Hub


## Gerar docker file


```bash
  docker build -t meu-servidor-apache .

```



## Executar o contêiner Docker
```bash
  docker run -d -p 80:80 meu-servidor-apache

```
    

## Subir no Docker Hub

Etapas:

```bash
  docker login

```
```bash
  docker tag meu-servidor-apache seu-usuario/meu-servidor-apache

```
```bash
  docker push seu-usuario/meu-servidor-apache

```

## Repositório Docker

 - [Docker](https://hub.docker.com/r/kopecode/meu-servidor-apache)
