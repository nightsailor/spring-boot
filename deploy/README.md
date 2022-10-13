2. Setting up and Building the Spring Boot Application

```pom.xml
<packaging>jar</packaging>

<build>
<plugins>
<plugin>
<configuration> 
		<executable>true</executable> 
</configuration>
```

3. Build the Spring Boot application
```
mvn clean package
```

4. Setting up Linux service

4.1 Create a service file

/etc/systemd/system/springboot.service

4.2 Create a symlink / Delete a symlink

sudo ln -s /software/tomcat/springboot.jar /etc/init.d/springboot

rm /etc/init.d/springboot

4.3 Update systemd

systemctl daemon-reload

4.4 Enable the service

systemctl enable springboot.service

4.5 Start the service

systemctl start springboot
systemctl stop springboot
systemctl restart springboot
systemctl status springboot
