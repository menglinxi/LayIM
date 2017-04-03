### SpringBoot-WebSocket

### required
* Scala 2.1+
* JDK 1.8+
* Gradle 3.+
* Mysql 5.1+

![功能设计](https://github.com/scalad/WebSocket/blob/master/doc/image/function.png)

### technology

* Gradle
* Scala
* SpringBoot
* SpringSecurity
* Spring Data Jpa
* Redis


### application.properties configuration
    
	# Datasource
	spring.datasource.url = jdbc:mysql://localhost:3306/websocket
	spring.datasource.username = root
	spring.datasource.password = root
	spring.datasource.driverClassName = com.mysql.jdbc.Driver
	
	# Spring MVC configration
	spring.mvc.view.prefix=/WEB-INF/view/
	spring.mvc.view.suffix=.jsp
	
	# Specify the DBMS
	spring.jpa.database = MYSQL
	# Show or not log for each sql query
	spring.jpa.show-sql = true
	# Hibernate ddl auto (create, create-drop, update)
	spring.jpa.hibernate.ddl-auto = update
	# stripped before adding them to the entity manager)
	spring.jpa.properties.hibernate.dialect = org.hibernate.dialect.MySQL5Dialect
	
	# Server port
	server.port=80
	
	# Redis Configration
	# Redis database index, default is 0
	spring.redis.database=0 
	spring.redis.host=120.27.114.229
	spring.redis.password=redis
	spring.redis.port=6379
	spring.redis.pool.max-idle=8
	spring.redis.pool.min-idle=0
	spring.redis.pool.max-active=8
	spring.redis.pool.max-wait=-1
	spring.redis.timeout=100
	
### build

* git clone https://github.com/silence940109/WebSocket.git
* gradle bootRun
* http://localhost:8080/swagger-ui.html