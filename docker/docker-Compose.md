# Docker-Compose
...

## Networking
By default Docker-Compose will create a new network for the given compose file. You can change the behavior by defining custom networks in your compose file.
### Create and assign custom network
...
*Example:*
```yaml
networks:
  custom-network:

services:
  app:
    networks:
      - custom-network
```
### Use existing networks
If you want to use an existing Docker network for your compose files, you can add the `external: true` parameter in your compose file
*Example:*
```yaml
networks:
  existing-network:
    external: true
```

## Volumes
Volumes allow Docker containers to use persistent storage. In a compose file, you can create and map volumes like this:
```yaml
volumes:
  my-volume:

services:
  app:
    volumes:
      - my-volume:/path-in-container
```

These volumes are stored in `/var/lib/docker/volumes`.


Docker Compose pour orchestrer vos conteneurs.

- docker-compose up -d vous permettra de démarrer l'ensemble des conteneurs en arrière-plan ;
- docker-compose ps vous permettra de voir le statut de l'ensemble de votre stack ;
- docker-compose logs -f --tail 5 vous permettra d'afficher les logs de votre stack ;
- docker-compose stop vous permettra d'arrêter l'ensemble des services d'une stack ;
- docker-compose down vous permettra de détruire l'ensemble des ressources d'une stack ;
- docker-compose config vous permettra de valider la syntaxe de votre fichier docker-compose.yml.
- docker-compose up --build -d

docker-compose up -d
docker-compose down --rmi all