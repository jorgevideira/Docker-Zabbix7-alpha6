# README

### Esse procedimento foi criado somente para fim de teste e conhecimento da nova versão do Zabbix 7 Alpha 6, não utilizar em produção.

A imagem do container foi criada utilizando: 

Ubuntu 22.04
Postgresql 14.9
Apache
Zabbix Server 7 Alpha 6.

1- Copie o arquivo do docker-compose.yaml e inicie o container. 

2 - Após iniciar o container, executar os seguintes comandos para iniciar os serviços do Zabbix e do postgresql.
 - docker exec -it zabbix /etc/init.d/postgresql start
 - docker exec -it zabbix /etc/init.d/apache2 start
 - docker exec -it zabbix /etc/init.d/zabbix-server start
 - docker exec -it zabbix /etc/init.d/zabbix-agent start
   
3- Acessar a interface web no endereço:
   http://localhost:8080/zabbix
