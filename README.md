# Example Micronaut Reactive Hibernate (with no Micronaut-data)

## A database in docker:

```shell
docker run -p 3306:3306 -e MYSQL_ROOT_PASSWORD=pass mysql:oracle
```

## Then run the app

```shell
./gradlew run
```

## Then test it!

```shell
❯ curl http://localhost:8080
[]%
❯ curl -X POST -d '{"name": "A genre"}' -H "Content-type: application/json" http://localhost:8080
{"id":1,"name":"A genre"}%
❯ curl http://localhost:8080
[{"id":1,"name":"A genre"}]%
```

## Then Grab a coffee, and celebrate!

☕️🥳 🎉

