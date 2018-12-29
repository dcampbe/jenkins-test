```sh
docker-compose -f .\docker-compose.test.yml build
export JENKINS_HOME=/path/to/jenkins/config
docker-compose config
docker-compose -f .\docker-compose.test.yml up
# things
docker login
docker image push dcamp/jenkins-test
```
