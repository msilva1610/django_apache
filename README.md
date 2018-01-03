# django_apache - Gileno Seção 7/82
###### Instalação de um django Server com base no apache2

###### Instalação do apache server 

```
sudo apt-get update
sudo apt-get install nginx
sudo apt-get install supervisor
sudo apt-get install python3-dev
```

###### Instalação do pip 
```
wget https://bootstrap.pypa.io/get-pip.py
```

# Hosting Django with apache server

###### Instalação do pip

```
sudo apt-get install python-pip
```

###### Instalação do apache
```
sudo apt-get install apache2
sudo apt-get install apache2-mpm-prefork
sudo apt-get install apache2-utils
sudo apt-get install libexpatl
```

A instalação do prefork está com probema

###### Instalação do módulo wsgi
```
sudo apt-get install libapache2-mod-wsgi
```

###### instalação do mysql server e o módulo client e as depêndencias

```
sudo apt-get install python-pip
sudo apt-get install libmysqlclient-dev
sudo apt-get install mysql-dev
sudo apt-get install mysql-server 
sudo apt-get install mysql-client
```
###### verifica e instala apenas o que está faltando

```
sudo apt-get install build-essential libmysqlclient-dev
```

###### instalar postgresql

```
sudo apt-get install postgresql 
sudo apt-get install postgresql-contrib
```

###### instalar o python-psycopg2

```
sudo apt-get install python-psycopg2
```

###### instalar o django

```
sudo pip install django
```

###### Colocando o usuário atual (ubuntu) como owner do /var/www

```
cd /var/www
sudo chown -R ubuntu .
sudo chmod -R g+w .
```

###### Criando um projeto no var/www

```
django-admin startproject Project
```

###### Verificar se tudo ok

```
cd Project
python manage.py migrate
```
###### Modificar as configurações do apache e permissões do usuário atual (ubuntu)

```
cd /etc/apache2
sudo chown -R ubuntu .
sudo chmod -R g+w .
```

###### Abrir a página de index do apache e verificar a configuração
> A configuração deve dizer que as configurações estão no apache2.conf na seção configuration overview


