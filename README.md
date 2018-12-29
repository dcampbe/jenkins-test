```sh
docker swarm init
docker-compose -f .\docker-compose.yml build
echo "admin" | docker secret create jenkins-user -
echo "admin" | docker secret create jenkins-pass -
export JENKINS_HOME=/path/to/jenkins/config
docker-compose config
docker stack deploy --compose-file=docker-compose.yml jenkins
# things
docker login
docker image push dcamp/jenkins-test
```
