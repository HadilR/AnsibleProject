# Déploiement automatique avec Ansible et Kubernetes

## Introduction

Ce projet vise à explorer deux outils modernes, largement utilisés par les administrateurs système, pour déployer un réseau de manière automatisée. Ces outils, Ansible et Kubernetes, trouvent leur place dans l'industrie pour le développement et les tests. La première partie du projet se concentre sur le déploiement automatique avec Ansible dans un environnement Linux natif, excluant l'utilisation de conteneurs. La seconde partie offre une rapide immersion dans Kubernetes, un puissant gestionnaire de conteneurs Docker flexible et en forte expansion.

## I - Ansible

Une start-up répartie sur deux sites géographiques doit concevoir et mettre en place son parc informatique. L'utilisation d'Ansible pour le déploiement automatique des services sur 4 machines virtuelles (2 par site) sous Debian est envisagée. Le projet s'inscrit dans une perspective d'automatisation maximale pour gérer efficacement des centaines de machines. Les besoins comprennent la mise en place de serveurs DHCP et DNS par site, un VPN pour interconnecter les deux sites, un NFS public et privé pour chaque utilisateur, un gestionnaire de dépôt Git, un serveur Apache, une authentification générale via LDAP, et une mise à jour globale des systèmes en une seule commande Ansible. L'objectif est de permettre l'ajout automatique d'un nœud dans le cluster avec quelques lignes de commandes Ansible.

## II - Découverte de Kubernetes

La seconde partie du projet se consacre à la découverte de Kubernetes, un gestionnaire de conteneurs simplifiant le déploiement et la gestion d'un cluster, y compris la répartition de la charge. L'étude initiale portera sur l'utilisation générale de Kubernetes. Ensuite, nous déploierons 4 instances Nginx (serveur web) dans des conteneurs Docker en utilisant Kubernetes. Cette étape permettra de comprendre comment Kubernetes facilite la gestion de conteneurs dans un environnement distribué.
