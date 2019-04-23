# Ansible
## Installation : 

Pour installer Ansible sur votre machine : https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html

Ensuite git clone de ce projet


## Modification des fichiers

* Dans le dossier `/host_vars/`  
	Remplacez dans chaques fichiers de conf `.yml` à la ligne ansible_host par chaque adresse ip de vos machine (si plusieurs machines)

* Dans `ansible.cfg` ajouter à la ligne`remote_user` le nom d'utilisateurs de vos machines
* Dans `playbook\playbook.yml` ajouter également à la ligne `remote_user` le nom d'utilisateurs de vos machines



# Lancement

Pour lancer l'installation des playbooks :

	> ansible-playbook /playbook/playbook.yml -i ./inventory.ini

