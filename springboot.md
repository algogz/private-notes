# Spring Boot notes

## spring-boot-admin
See https://github.com/codecentric/spring-boot-admin

An excellent UI to view information from spring-boot-acuator.

## shiro integration
See https://github.com/algogz/Spring-Boot-Shiro

## build-info
To have the version show up in the application list you can use the build-info goal from the spring-boot-maven-plugin, 
which generates the `META-INF/build-info.properties`. See also the Spring Boot Reference Guide.

pom.xml
```
<build>
    <plugins>
        <plugin>
            <groupId>org.springframework.boot</groupId>
            <artifactId>spring-boot-maven-plugin</artifactId>
            <executions>
                <execution>
                    <goals>
                        <goal>build-info</goal>
                    </goals>
                </execution>
            </executions>
        </plugin>
    </plugins>
</build>
```
