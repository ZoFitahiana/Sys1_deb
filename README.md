<div style="text-align: center;">
                                <span style="color: red;">

# Automatisation de la configuration des Virtual Hosts avec Ansible

</span>
</div>
Ce script Ansible permet d'automatiser la configuration des Virtual Hosts d'Apache                                      en utilisant un fichier YAML pour spécifier les noms de domaine et effectuer les                                    modifications nécessaires dans les fichiers de configuration.
<div>
<span style="color: white;">

## Prérequis :

</span>
</div>

<p>Ansible doit être installé sur la machine à partir de laquelle vous allez exécuter le script.</p>
<p>Si Apache n'est pas déjà installé, le script se chargera de son installation.</p>

<span style="color: white;">

## Utilisation :

</span>

 1- Assurez-vous que vous avez les droits d'accès et les permissions appropriés pour exécuter des tâches administratives sur les machines cibles.
 2- Clonez ce dépôt Git sur la machine à partir de laquelle vous souhaitez exécuter le script.
 3- Modifiez le fichier `config.yml` avec les noms de domaine souhaités pour les Virtual Hosts. 
 4- Exécutez le script Ansible en utilisant la commande suivante : `$ansible-playbook playbook.yml`.                   Le script se chargera d'installer Apache (si nécessaire), de créer les dossiers pour les Virtual Hosts spécifiés et de modifier les fichiers de configuration d'Apache en conséquence.         
 5- Vérifiez les résultats pour vous assurer que les Virtual Hosts ont été configurés correctement.

<span style="color: white;">

## Personnalisation :

</span>

.Vous pouvez personnaliser les répertoires des Virtual Hosts en modifiant le chemin `directory` dans le fichier `config.yml`.
.Si vous avez des configurations spécifiques pour chaque Virtual Host, vous pouvez ajouter les tâches nécessaires dans le fichier `playbook.yml`.



