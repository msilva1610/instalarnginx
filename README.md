# Passos para instalar nginx
## Centos7

Atualizar o repositório de pacotes do centos

```
yum -y update
```

Instalar o EPEL repository
```
yum install epel-release -y
```

#### Instalar o nginx

```
yum install nginx -y
```


#### Instalar os pacotes de apoio
```
yum install git wget curl vim nano -y
