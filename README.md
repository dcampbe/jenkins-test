```sh
docker swarm init
echo "admin" | docker secret create jenkins-user -
echo "admin" | docker secret create jenkins-pass -
docker stack deploy --compose-file=docker-compose.yml jenkins
```
