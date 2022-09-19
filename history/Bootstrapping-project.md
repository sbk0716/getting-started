## 0. Prerequisite
* Install Apache Maven
* Install Azul JDK(for Apple Ailicon Mac)

# 1. Bootstrapping the project
```sh
% mvn io.quarkus.platform:quarkus-maven-plugin:2.12.2.Final:create \
    -DprojectGroupId=org.acme \
    -DprojectArtifactId=getting-started \
    -Dextensions="resteasy-reactive"
...
...
% ls getting-started 
README.md       mvnw.cmd        src
mvnw            pom.xml         target
% 
```

# 2. Running the application
```sh
% ./mvnw quarkus:dev
```

# 3. Packaging and run the application
```sh
% ./mvnw clean package
% java -jar target/quarkus-app/quarkus-run.jar
```


# 4. Reference
* https://quarkus.io/guides/getting-started
