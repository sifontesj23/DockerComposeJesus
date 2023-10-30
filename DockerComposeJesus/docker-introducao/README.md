
## Como rodar

### Instalando dependências
Acesse a pasta `./api` no terminal e execute:
```
npm install
```

Com isso instalamos as dependências Node que precisamos. Estou utilizando Node 10.


### Rodando os containers e descarregando images com docker-compose up -d

Na pasta raíz do projeto, execute:

docker-compose up -d

### Agora faça o restore do banco:
```
Linux: docker exec -i mysql-container mysql -uroot -pprogramadorabordo < api/db/script.sql
wimdons: cat api/db/script.sql | docker exec -i mysql-container mysql -uroot -pjesus
```
