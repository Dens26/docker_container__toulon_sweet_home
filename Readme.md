# DOCKER CONTAINER HOME SWEET HOME

Container de developpement pour l'application Home Sweet Home.

Ce container contient :
- Un serveur apache
- Une base de données Mysql
- Un serveur phpMyAdmin


### MISE EN PLACE

Création du container
```
>   docker-compose up -d
```

Liste des services en cours
```
>   docker -ps
```

### BASH

- Ouvrez le dossier et tapez :

```
docker exec -it <id du service server> bash
```

Vous vous retrouvez dans le dossier www

Pour supprimer le fichier html si pas d'utilité
```
rm -r html
```

### INSTALLER SYMFONY
[Documentation](https://symfony.com/doc/current/index.html)

Initialisation des composant symfony
```
composer create-project symfony/skeleton:"7.0.*" project
```

Allez dans le projet nouvellement créé
```
cd project
```

Instalation des composants
```
composer require webapp
```
