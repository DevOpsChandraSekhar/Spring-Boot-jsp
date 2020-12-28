# Springboot with jsp application
  Technologies used :

  1. Spring Boot 2.4.1 RELEASE
  2. Spring 4.3.4.RELEASE
  3. Tomcat Embed 8.5.6
  4. Maven 3
  5. Java 8
 
# Do the following changes manually
 
 1. Create the following folders manually :
   *webapp and subfolders
   
 2. Project Dependencies
    <!-- Tomcat embedded container -->
		<dependency>
			<groupId>org.springframework.boot</groupId>
			<artifactId>spring-boot-starter-tomcat</artifactId>
			<scope>provided</scope>
		</dependency>

		<!-- JSTL for JSP -->
		<dependency>
			<groupId>javax.servlet</groupId>
			<artifactId>jstl</artifactId>
		</dependency>

		<!-- Need this to compile JSP -->
		<dependency>
			<groupId>org.apache.tomcat.embed</groupId>
			<artifactId>tomcat-embed-jasper</artifactId>
			<scope>provided</scope>
		</dependency>

		<!-- Need this to compile JSP, tomcat-embed-jasper version is not working, 
			no idea why -->
		<dependency>
			<groupId>org.eclipse.jdt.core.compiler</groupId>
			<artifactId>ecj</artifactId>
			<version>4.6.1</version>
			<scope>provided</scope>
		</dependency>
		
 3. This SpringBootServletInitializer run a SpringApplication from a traditional WAR deployment
 
 4. A simple Spring controller class.
 
 5. JSP + Resources + Static files 
    * src/main/webapp/WEB-INF/jsp/
 6. For static files like CSS or Javascript, put in 
    * /src/main/resources/static/
 7. For properties files, put in 
    * /src/main/resources/
 8. Start the Spring Boot web app and Access 
    http://localhost:8080

