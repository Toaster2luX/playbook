Plaubook pour changer le serveur de temps 

Ajouter les hosts dans le fichier inventory
Changer la valeur du serveur ntp dans chrony.yml

execution
$ ansible-playbook -i inventory/hosts playbook/chronyd.yml -e "srv_ntp=192.168.3.53" -Kk
