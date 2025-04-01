# WIK-DPS-TP02

Pour démarrer le projet, il faut:
```
git clone https://github.com/Orealyz/TP2-Devops-Ynov.git
```

Se rendre dans le dossier api:
```
cd /api
```

Démarrer le docker compose:
```
docker compose up-d 
```

Ensuite:
```
curl http://localhost:8080/ping
```

Et vérifier dans les logs que le loadbalancer est bien effectué:
```
docker compose logs -f api
```

Enjoy :)
