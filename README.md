# AnsibleProject

1) Set up de l'environnement :

creation de deux sous reseaux: intnet et intnet2
1er sous-reseau : vm-ansible (server base)   192.168.10.101
			      vm1-1   192.168.10.10
			      vm1-2   192.168.10.20

2eme sous-resau : vm2-1    192.168.20.10
		  vm2-2    192.168.20.20
dans chaque machine on doit installer openssh et python3
Pour que la machine ansible peut communiquer avec internet (pour l'installation de ansible etc et aussi pour communiquer avec les autres machines de sous reseaux), on a crée un routeur :
dans le routeur on a 4 interfaces : Nat (pour internet)
				    192.168.10.1
				    192.168.20.1
on a configuré le nat pour laisser passer que le trafic de machine vm-ansible (forward & postrouting)
il faut regarder historique chagpt pour les commandes

2) on connecte la machine ansible avec les autres machines via ssh (keys etc)

3) on a crée ce repository pour enregistrer notre travail
4) dans ce repository on a crée le fichier inventory(on met dedans les adresses destinations)
5) on fait un ping avec cette commande : 
ansible all --key-file ~/.ssh/ansible -i inventory -m ping 
6) on crée un fichier ansible.cfg on configure dedans le inventory et la cle ssh pour minimiser la commande ping : ansible all -m ping 

