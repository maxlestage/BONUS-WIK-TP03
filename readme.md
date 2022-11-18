# TP-WIK-DPS-TP03-BONUS

## CONSIGNES :

Créer un docker-compose.yaml pour déployer une architecture 3 tiers (app/db/front):

- Un wordpress répliqué au moins 2 fois ✅
- Une base de données mysql ✅
- Une base de données de cache redis ✅
- Un reverse proxy nginx pour servir le wordpress (le seul service exposé) ✅
- Configurer wordpress pour utiliser les différents services ✅

## Les Technos :

- WordPress
- Mysql
- Redis

## Lancer le projet :

Commande à lancer dans le temrinal à la racine du projet :

```rs
docker compose up // Affiche l'état de l'app avec le serveur démarré, ainsi que l'action du server balancing.
```

Nous pouvons ainsi voir que la base Mysql ainsi que Redis, le proxy NGINX et le Wordpress se lance correctement:
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/Debug_capture_vscode1.png)

Ensuite on installe le plugin Redis Cache pour WordPress de "Till Krüss"
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/Redis_ext_wp.png)

Une fois l'extension installée, on l'active, puis on retrouve l'état de celle-ci:
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/WP_Etat_de_connexion1.png)
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/WP_Etat_de_connexion2.png)
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/WP_Etat_de_connexion3.png)

Redis est donc bien installé, on peut maintenant visiter le wordpress pour y laisser un commentaire par exemple:
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/WP_test_comment1.png)
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/WP_test_comment2.png)

En revenant dans VScode, on remarque que tout se passe correctement, redis est bien relié et fait le travail:
![screenshot](https://github.com/maxlestage/BONUS-WIK-TP03/blob/main/images/Debug_capture_vscode1.png)

LESTAGE Maxime - TP DevOps n°3 - BONUS - Ynov 2022.
