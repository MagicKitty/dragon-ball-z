# 1 - Introduction à Docker

### Docker

Installez docker sur vos machines.
Il s'agit d'un logiciel principalement disponible sur linux, sur windows et macOS il est plus difficilement installable car il faut virtualiser linux.

On va commencer par lancer l'image "hello-world".

Puis on va lancer une image Linux légère. Entrez dans le conteneur et éditez un fichier nommé "hello.txt" avec écrit à l'intérieur "Welcome to DBZ !" dans n'importe quel répertoire. Sortez du conteneur et visualisez le contenu du fichier depuis le CLI.

Maintenant on lance MySQL et PostgreSQL.

Trouvez et supprimez les conteneurs docker. Imaginez qu'il existe 100 conteneurs, comment feriez-vous ce travail ?

On résume :
Une image est utilsée lors du lancement d'un conteneur. Une fois le conteneur lancé, il devient accessible via le docker CLI. Comme vous l'aurez sans doute remarqué, il existe plusieurs façon d'obtenir un même résultat. Un fois qu'un conteneur a été lancé, par défaut il va s'éteindre si on ne lui précise pas de rester ouvert.

Ne visualisez pas docker et ses conteneurs comme des instances précieuse à ne surtout pas supprimer. C'est justement tout le contraire. Un conteneur doit pouvoir être down quand on le veut. Et remplaçable par un autre très rapidement (montée en version). On créé un environnement propice à l'exécution d'un certain bout d'application. Lorsqu'on en veut plus on peut changer le code et garder le même environnement. On a ainsi un environnement parfaitement ISO sur toutes les machines du monde. Un conteneur docker qui utilise une certaine image fonctionnera de la même manière sur Namek comme sur la Terre. (Version de dev/pre-prod/prod ISO sur tous serveurs). On fait disparaître la problématique du "Works on my machine" qui date de l'époque des disquettes et des CD-ROM !

Note supplémentaire :
Les images se situent sur le docker hub. Il en existe des tas, allant de OracleSQL à MongoDB, ou de Windows à Linux. Jettez un oeuil si vous avez un doute sur le nom d'une image.
Par défaut la version est à "latest", mais vous pouvez choisir la version que vous voulez.

### Tomcat/Nginx

Lancez un conteneur tomcat avec le docker CLI sur le port 9876. Lancez votre navigateur sur localhost:9876.

Lancez maintenant nginx sur un autre port. Cette fois-ci, trouvez un moyen de fermer le terminal sans couper nginx. Testez sur votre navigateur.

Remplacez le fichier index.html par défaut dans nginx par celui qui a été mis à disposition.



On a terminé pour aujourd'hui !
