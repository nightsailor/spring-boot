1. Add Maven Plugin to POM.XML

```pom.xml
<build>
<plugins>
  <plugin>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-maven-plugin</artifactId>
  </plugin>
</plugins>
</build>
```

2. Build Spring Boot Project with Maven
```
mvn clean package
```
or
```
mvn package
```
or
```
mvn install / mvn clean install
```

3. Run Spring Boot app using Maven:
```
mvn spring-boot:run
```

4. [optional] Run Spring Boot app with java -jar command
```
java -jar target/mywebserviceapp-0.0.1-SNAPSHOT.jar
```

5. Debug

```
$ readlink -f $(which java)
/usr/lib/jvm/java-17-openjdk-amd64/bin/java
$ echo $JAVA_HOME
/usr/lib/jvm/java-11-openjdk-amd64
$ java -version
$ javac -version
$ export JAVA_HOME=xxxxxx
```