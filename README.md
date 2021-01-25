# 1 - Introduction à Docker

### Docker

Pour cette partie je conseil une image linux qui se nomme Alpine.

La commande `run` est un raccourcis pour `create` + `start`.

La commande `exec` est intéressante lorsque vous souhaitez exécuter une commande dans un conteneur. Il faut que la commande soit connue dans le conteneur pour qu'elle fonctionne.

Pour créer un fichier, vous avez à disposition dans le shell linux d'Alpine la commande `echo`. Il y a une petite astuce qui permet de garder un conteneur en route après en être sorti.

Je propose le signe `$` dans le bash pour vous aider à supprimer les conteneurs.

### Tomcat/Nginx

Par défaut la page servie par nginx se situe dans `/usr/share/nginx/html`
