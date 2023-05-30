# Projeto conversão de temperatura

### Sobre o projeto
O projeto conversão de temperatura é um projeto desenvolvido em NodeJS. O projeto tem como objetivo ser um exemplo para a criação de ambiente com containers usando NodeJS.

### Observações do projeto
A aplicação é exposta usando a porta 8080

# Docker - C:\conversao-temperatura\ubuntu-curl>
docker build -t angelicabayer/aula-ubuntu-curl:v1 -f Dockerfile .
docker image ls
docker container run -it aula-ubuntu-curl
docker image prune (unused image)

# Docker C:\conversao-temperatura\src>
docker build -t angelicabayer/aula-conversao-temperatura:v1 .
docker image ls
docker image prune (unused image)
docker container run -d -p 8080:8080 angelicabayer/aula-conversao-temperatura:v1
docker container ls
 
# Subir a imagem para hub docker
docker login
docker push angelicabayer/aula-conversao-temperatura:v1
docker tag angelicabayer/aula-ubuntu-curl:v1 angelicabayer/aula-ubuntu-curl:latest

# Pipeline
[ ] Jenkins
[ ] GiLlab
[x] Git hub actions (https://github.com/angelicacamboim/conversao-temperatura/actions/new)

# Sites
https://codenotary.com/blog/extremely-useful-docker-commands