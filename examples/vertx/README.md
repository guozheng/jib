# Containerize a [Eclipse Vert.x](https://vertx.io/) application with Jib

This is an example of how to easily build a Docker image for a [Eclipse Vert.x application](https://vertx.io/) with Jib.

## Build directly to a Docker daemon:
```shell
./gradlew jibDockerBuild

docker run -d --rm -p 8080:8080 vertx-jib-example
```

## Publish to Image Registry
See: [publish to container registry](https://github.com/GoogleContainerTools/jib/tree/master/jib-gradle-plugin#Configuration) for more details
```shell
./gradlew jib
```

## More information

Learn [more about Jib](https://github.com/GoogleContainerTools/jib).

Learn [more about Eclipse Vert.x](https://vertx.io).
