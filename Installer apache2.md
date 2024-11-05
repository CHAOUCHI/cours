# Guide - Installer un serveur web sous Linux

## Pré-requis

- Debian (GNU/Linux)
- Le gestionnaire de paquet : `apt`

## Installer le paquet `apache2`

![alt text](image.png)

```bash
sudo apt install apache2
```


> `Attention` ! N'oubliez pas d'utiliser sudo pour passer en super-user lors de l'installation de apache2.


## Lancer le programme apache2

```bash
sudo systemctl start apache2
```

### Vérifier l'etat du serveur web avec systemd

```mermaid
flowchart
systemd
apache2
mysqld

systemd--->apache2
systemd--->mysqld
systemd--->kdeplasma

```
