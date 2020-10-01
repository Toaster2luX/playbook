Stopper le service et le supprimer du demarrage automatique selon la version de la distribution Centos 6 et 7


Sur un environnement sans bastion executer la commande
$ ansible-playbook -i inventories/hosts playbook_ossec.yml -K

Sur un environnement avec bastion executer la commande
$ ansible-playbook -i inventories/hosts playbook_ossec.yml -e '@inventories/bastion' -K


Pour le bastion remplacer les valeurs suivantes
nom du bastion
hostbastion

port du bastion
-p2222
