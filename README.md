###### README

# Bienvenue dans README.md

## B A S H

````bash
sudo apt update
sudo apt upgrade
````

# commande pour créer un utilisateur
````bash
sudo adduser nom_utilisateur
````
# commande pour ajouter un utilisateur au groupe sudo
````bash
sudo usermod -aG sudo nom_utilisateur
````
# voir le groupe sudo
````bash
sudo grep '^sudo' /etc/group
````

##############################
## ufw firewall configuration ##
##############################
sudo apt install ufw

## allow ipv6 "IPV6=yes"
sudo nano /etc/default/ufw
## default rules
sudo ufw default deny incoming
sudo ufw default allow outgoing
## allow ssh
sudo ufw allow ssh
## allow port xx
sudo ufw allow xx
## enable ufw
sudo ufw enable
## check ufw status
sudo ufw status verbose
## allow http
sudo ufw allow http
## allow https
sudo ufw allow https
## allow port 80
sudo ufw allow 80
## deny port 22/tcp
sudo ufw deny 22/tcp
## delete rule x
sudo ufw status numbered
sudo ufw delete x

## allow in x
sudo ufw allow in x
## allow out x
sudo ufw allow out x

## allow from ip_address
sudo ufw allow from ip_address

## vim
# delete all
:%d
# save & quit
:wq

