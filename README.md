# Curso Kubernetes - Udemy

##  Sobre o Projeto 

Projeto realizado conforme proposto no curso da Udemy :  ***Orquestração de Containers com Kubernetes***
link do curso -  https://www.udemy.com/course/orquestracao-de-containers-com-kubernetes/

### Resumo Aplicação

Simulado uma primeira aplicação onde é realizado uma votação de escolha entre Gato e Cachorro.
A segunda aplicação é onde conseguimos fazer a contagem desses votos.

### Objetivo

Utilizando a ferramenta de orquestração Kubernetes, foram criadas de forma declarativas alguns scripts no formato YAML para a criação de Deployments, Namespace e Services.

***Scripts disponíveis no path***: curso_k8s/secao_7/



#### Ferramentas utilizadas durante o curso

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

Nesta etapa conseguimos identificar os objetos existentes (PODS,DEPLOY,SERVICES,REPLICASETs) e seus devidos status.

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/5.1-%20verificando-namespace.png)

### Verificando o Ip de acesso ao serviço - Result

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/6-verificando-result-ip.png)

### Verificando o Ip de acesso ao serviço - Vote

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/7-verificando-vote-ip.png)

### Verificando a aplicação aonde realiza a votação
- Nesta etapa foram simulados 2 votos

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/8-open-app-votacao.png)

### Verificando o resultado a votação
- Nesta etapa conseguimos verificar o resultado da votação

![alt text](https://github.com/GumaFernando/curso_k8s/blob/master/imagens/9-consulta-votos.png)



# Como executar o projeto
 
 ***//pré-requisitos de softwares//***
 - Docker Hub
 - Minikube
 - Kubectl
 

- Faça o download dos scripts do path: curso_k8s/secao_7/
- Abra o Minikube via CMD e start o cluster
  command: minikube start --driver=docker
  
- Execute o script dentro do path: curso_k8s/secao_7/namespaces/
  command : kubectl apply -f votes.yaml --record
  
- Execute o script dentro do path: curso_k8s/secao_7/deploy/
  command : kubectl apply -f . --record 
  
- Execute o script dentro do path: curso_k8s/secao_7/services/
  command : kubectl apply -f . --record 
  
  
 ### Consultar no namespace -> vote os objetos criados e status
 
 kubectl get all -n vote
