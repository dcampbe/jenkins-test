Notes on how to CI this project:

```sh
docker-compose -f docker-compose.test.yml build
docker-compose up -d
docker-compose -f docker-compose.text.yml run sut
docker-compose down
```
