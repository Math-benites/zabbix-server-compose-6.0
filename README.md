<h1 align="center">Zabbix - Compose </h1>

### Pré-requisitos

Antes de começar, você vai precisar ter instalado 
[Ubuntu 22.04 LTS ](https://releases.ubuntu.com/jammy/)

[Docker Compose version v2.3.3 igual ou superior]

[Docker Engine Version: 23.0.1 igual ou superior]



### 🎲 ( Rodando Compose )

```bash
# Criando diretorios
$ mkdir -p /opt/app/
```
```bash
# Acessando diretorio
$ cd /opt/app
```
```bash
# Fazendo Git do projeto
$ git clone https://github.com/Math-benites/zabbix-compose-6.0.git . 
```
```bash
# Rodando compose
$ docker compose up -d
```

O servidor Zabbix inciará na porta:80 - acesse <http://MYIP/>

O servidor Grafana inciará na porta:3000 - acesse <http://MYIP:3000>

### 🔧 ( Alterando Configuracoes - Opicional )

```bash
# Zabbix server.config
$ nano ./zabbix/env_vars/.env_srv
```
```bash
# Zabbix web.config
$ nano ./zabbix/env_vars/.env_web
```
```bash
# Zabbix mysql.config
$ nano ./zabbix/env_vars/.env_db_mysql
```


