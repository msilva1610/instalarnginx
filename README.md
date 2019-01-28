# Passos para instalar nginx
## Centos7

#### Atualizar o repositório de pacotes do centos

```
yum -y update
```

#### Instalar o EPEL repository
```
yum install epel-release -y
```

#### Instalar o nginx

```
yum install nginx -y
```


#### Iniciando o nginx
```
systemctl start nginx
systemctl enable nginx
systemctl status nginx
```

#### Liberando o firewall

```
systemctl enable firewalld
systemctl start firewalld
systemctl status firewalld
firewall-cmd --zone=public --permanent --add-service=http
firewall-cmd --zone=public --permanent --add-service=https
firewall-cmd --reload
```

#### Instalar os pacotes de apoio
```
yum install git wget curl vim nano -y

## Outros comandos de apoio

Permitir usuário local de gravar no arquivo

```
chmod 744 arquivo
```

Exemplo de login na OCI com ssh

```
ssh -i id_rsa opc@ip
```

