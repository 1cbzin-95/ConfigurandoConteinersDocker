# ConfigurandoConteinersDocker  
mysql OU MARIADB  
```docker run --name mysql -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql
docker exec -it mysql_db bash
mysql -u root -p
```  

-- Baixar imagems --
```  
docker pull mongo
```

-- Visulizar as images Baixadas --
```  
docker images
```

-- Criar Conteiner da imagem escolhida --
```  
docker run --name mongo_db -p 27017:27017 -d mongo
```

-- Verificar quem esta rodando --
```  
docker ps -a
```

-- Como acessar o conteiner mongo --
                 nome_criado        usuario
```  
docker exec -it mongo_db  mongo   admin
```

-- Começar de rodar --
```  
docker start mongo_db
```

-- Parar de rodar --
```  
docker stop mongo_db
```

--REMOVER CONTAINER NO DOCKER
```  
docker rm mongo_db
```

--REMOVER IMAGES NO DOCKER
```  
docker rmi mongo
```
-----------------------------------POSTGRESS-----------------------------------  
Baixar a imagem do posgress
```  
sudo docker pull postgres 
```  
criar container do postgres e passando senha
```  
docker run --name postgres_db -e POSTGRES_PASSWORD=postgres -d -p 5432:5432 postgres   
``` 
Executar dentro do container
```  
docker exec -it postgres_db psql -U postgres --password |executar no conteiner
```








export PATH=$PATH:/home/cadubrito/sonar-scanner/bin

