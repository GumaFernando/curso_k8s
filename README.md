# - Curso Kubernetes - Udemy

##  Sobre o Projeto 

Projeto realizado conforme proposto no curso da Udemy : 

Utilizando a ferramenta de orquestração Kubernetes, foram criadas de forma declarativas, scripts no formato YAML para a criação de Deployments, Namespace e Services.

#### Ferramentas utilizadas no curso

- Minikube 
- Docker Hub
- VsCode

## Desenvolvimento

### Start no cluster

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/1-start-cluster.png)

### Verificando os namespaces existentes
  Obs: Não temos o namespace ***vote*** criado !
  
  ![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/2-get-namespaces.png)
  
### Criando o namespace -> Vote

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/3-criando-ns.png)

### Criando os deployments 

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/4%20-%20criando-deploy.png)

### Criando os serviços

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/5-criando-services.png)

### Verificando os objetos existentes dentro do namespace -> VOTE

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/5.1-%20verificando-namespace.png)

### Verificando o Ip de acesso ao serviço - Result

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/6-verificando-result-ip.png)

### Verificando o Ip de acesso ao serviço - Vote

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/7-verificando-vote-ip.png)

### Verificando a aplicação aonde realiza a votação

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/8-open-app-votacao.png)

### Verificando o resultado a votação

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/9-consulta-votos.png)
