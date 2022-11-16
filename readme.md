# TP-WIK-DPS-TP03-BONUS

## CONSIGNES :

Créer un docker-compose.yaml pour déployer une architecture 3 tiers (app/db/front):

- Un wordpress répliqué au moins 2 fois
- Une base de données mysql
- Une base de données de cache redis
- Un reverse proxy nginx pour servir le wordpress (le seul service exposé)
- Configurer wordpress pour utiliser les différents services

## Les Technos :

- WordPress
- Mysql
- Redis

## Lancer le projet :

Commande à lancer dans le temrinal à la racine du projet :

```rs
docker compose up // Affiche l'état de l'app avec le serveur démarré, ainsi que l'action du server balancing.
```

```rs
docker inspect $(docker ps -q) --format '{{.Config.User}} {{.Name}}' // Permet de visualiser l'utilisateur, dans notre cas on run avec "userapi"
```

LESTAGE Maxime - TP DevOps n°3 - BONUS - Ynov 2022.
