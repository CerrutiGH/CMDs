<h1 align="center"> Terminal Commands </h1>

<h3>Docker</h3>

<p>docker containner run --name [nome][imagem] -> Criar container</p>

<p>docker container ls -a -> Listar containers desativados</p>

<p>docker container rm [nome/id] -> Excluir container</p>

<p>docker container rm -f [nomeid] -> Força a exclusão de um container</p>

<p>docker container run --name [nome] --rm [imagem]</p>

<p>docker container run -it [imagem] /bin/bash -> Modo interativo do container</p>
  
<p>docker container run nginx -> Container contínuo</p>
  
<p>docker container run -d nginx -> Container contínuo em modo dimon (Segundo plano)</p>
  
<p>docker container run -d -p [porta local]:[porta container] -> Fazer um port</p>
  
<p>docker container run -d -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=mongouser -e MONGO_INITDB_ROOT_PASSWORD=mongopwd mongo -> Iniciando mongo db com Environment Variable (Verificar no docker hub)</p>
  
<p>docker container inspect [nome/id] -> Gera uma estrutura Json com informações do container</p>
  
<p>docker container exec -it [nome/id] -> Acesso ao terminal do container</p>
  
<p>docker stop [nome/id] -> Para execução do container</p>
  
<p>docker start [nome/id] -> Começar execução do container</p>
  
<p>docker container logs [nome/id] -> verificação de logs</p>
  
<p>docker container logs -n [numero] [nome/id] -> verificação das ultimas [numeros] linhas</p>
  
<p>docker container logs -f [nome/id] -> verificação de logs continuamente</p>
  
<p>docker container logs -t [nome/id] -> verificação de logs e data e tempo</p>
  
<p>docker commit [nome/id] [nome imagem] -> Faz uma copia da imagem de outra imagem ja existente</p>
  
<p>docker image ls -> Listar Imagens</p>
  
<p>docker image build -t [nome] "[caminho em que se encontra o Dockerfile]" -> Construção de imagem a partir de um Dockerfile</p>
  
<p>docker image prume -> Tira as imagens sem uso e referencia</p>
  
<p>docker image rm [nome/id] -> Exclui uma imagem </p>
  
<p>docker image inspect [nome/id] -> Gerar informações da imagem</p>
  
<p>docker image history [image/nome] -> Gera historico de uso da imagem associada</p>
  
<p>docker login</p>
  
<p>docker tag [imagem] YOUR_DOCKERHUB_NAME/[imagem]</p>
  
<p>docker push [nome imagem]</p>

</br>

<h3>Terraform</h3>
<p>terraform init  -> Baixar os providers declarados</p>

<p>terraform plan  -> Mostra a infra que está sendo implantada</p>

<p>terraform apply -> Implantação do recurso</P>

</br>

<h3>Kubernetes</h3>
<p>kubectl version --client</p>

<p>kubectl clusterindo dump </p>

<p>kubectl api-resources -> Verifica recursos e suas versões</p>

<p>kubectl api-resources | grep/findstr replicaset -> Verifica recursos e suas versões filtrando pelo nome</p>

<p>kubectl create -f meupod.yaml</p>

<p>kubectl apply -f meupod.yaml</p>

<p>kubectl get nodes</p>

<p>kubectl describe pod meupod</p>

<p>kubectl port-forward pod/meupod 8080:80</p>

<p>kubectl get pods</p>

<p>kubectl get pods -l app=web</p>

<p>kubectl delete pod meupod</p>

<p>kubectl rollout history deployment [nome do deployment] > Ver versões anteriores</p>

<p>kubectl rollout undo deployment [nome do deployment] -> Volta pra versão anteriores</p>
