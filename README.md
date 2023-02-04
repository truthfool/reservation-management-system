# ReservationSystem

An reservation system where users/residents can log in and reserve a time to use a service such as fitness center, pool, or sauna in a hypothetical apartment complex. Each amenity will have a certain capacity (number of people that can use the service at the same time) so that people can make use of the amenities safely during the Covid-19 pandemic.

Technologies
- Spring Boot
- Thymeleaf 
- Hibernate 
- Swagger 
- Spring Security 
- Maven 
- JPA 
- H2 In-Memory Database 
- Bootstrap


## Development

During development it is recommended to use the profile `local`. In IntelliJ, `-Dspring.profiles.active=local` can be added in the VM options of the Run Configuration after enabling this property in "Modify options".

Update your local database connection in `application.yml` or create your own `application-local.yml` file to override settings for development.

Lombok must be supported by your IDE. For this, in IntelliJ install the Lombok plugin and enable annotation processing - [learn more](https://bootify.io/intellij/spring-boot-with-lombok.html).

After starting the application it is accessible under `localhost:8080`.

## Build

The application can be built using the following command:

```
mvnw clean package
```

The application can then be started with the following command - here with the profile `production`:

```
java -Dspring.profiles.active=production -jar ./target/reservation-system-0.0.1-SNAPSHOT.jar
```

## Further readings

* [Maven docs](https://maven.apache.org/guides/index.html)  
* [Spring Boot reference](https://docs.spring.io/spring-boot/docs/current/reference/htmlsingle/)  
* [Spring Data JPA reference](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/)  
