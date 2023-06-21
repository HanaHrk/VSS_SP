# Prerequisite

## Database

You have to start **MariaDB** database with user **rest-benchmark** and password **rest-benchmark** with created **VSS** scheme. MariaDB server must listen on port **3306** and must be called from **localhost** address. In other cases, you have to check each program documentation for parameters change.



## Running

### Spring Boot

#### Prerequisite

- Gradle

- Java 11+

  

Copy **Spring Boot** folder on the server with:

```console
sudo scp -r Spring\ Boot 185.177.116.187:/home/tmp
```

In project root directory run:

```console
./gradlew bootBuildImage — imageName=springbootbenchmark
docker compose up
```

