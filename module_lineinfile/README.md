# Module LineInFile
-----------------
Pour ajouter une ligne dans un fichier
Pour mon besoin, necessite l'ajout de 3 variables 

* prenom
* nom
* certificat


## Exécution
-----------------
Pour le test en local
* $ ansible-playbook -i hosts playbook_localtest.yml -e "prenom=John nom=Doo certificat=11111DDD"

Pour les serveurs apache distants
* $ ansible-playbook -i hosts playbook_lineinfile.yml-e "prenom=John2 nom=Doo2 certificat=11111BBB" -e "destination=workspace1"

Pour un prénom/nom composé, le mettre en simple cote ''
* $ ansible-playbook -i hosts playbook_lineinfile.yml-e "prenom='John3 JR' nom=Doo3 certificat=11111AAA" -e "destination=workspace1"

 

