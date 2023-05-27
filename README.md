###### README

# Bienvenue dans README.md

## B A S H

````bash
sudo apt update
sudo apt upgrade

## commande pour créer un utilisateur
sudo adduser nom_utilisateur
## commande pour ajouter un utilisateur au groupe sudo
sudo usermod -aG sudo nom_utilisateur

## voir le groupe sudo
sudo grep '^sudo' /etc/group

## ufw firewall configuration
sudo apt install ufw

## allow ipv6 "IPV6=yes"
sudo nano /etc/default/ufw
## default rules
sudo ufw default deny incoming
sudo ufw default allow outgoing


sudo ufw status verbose
sudo ufw enable
