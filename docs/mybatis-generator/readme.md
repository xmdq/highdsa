## mybatis-generator 自动生成PO类、mapper文件、Dao接口类
***
### 文档说明
**通过使用mybatis-generator来自动生成PO类、mapper文件、Dao接口类**   

[快速开始链接](http://www.mybatis.org/generator/quickstart.html)

自动生成之前，需要检查以下几项：
1. 将这两个配置文件放到某个工程下,generatorConfig.xml默认加载classpath下的generator-mysql.properties,同时需要检查resources的build path;
2. 检查generator-mysql.properties中mappers子目录是用包的点形式还是目录下划线;
3. 加入mybatis和相应的数据库jar包,如

	<dependency>
		<groupId>org.mybatis</groupId>
		<artifactId>mybatis</artifactId>
		<version>3.4.5</version>
	</dependency>
	<dependency>
		<groupId>mysql</groupId>
		<artifactId>mysql-connector-java</artifactId>
		<version>5.1.45</version>
	</dependency>
	<!-- 可选日志 -->
	<dependency>
		<groupId>org.apache.logging.log4j</groupId>
		<artifactId>log4j-api</artifactId>
		<version>2.9.0</version>
	</dependency>
	<dependency>
		<groupId>org.apache.logging.log4j</groupId>
		<artifactId>log4j-core</artifactId>
		<version>2.9.0</version>
	</dependency>
	<dependency>
		<groupId>org.apache.logging.log4j</groupId>
		<artifactId>log4j-slf4j-impl</artifactId>
		<version>2.9.0</version>
	</dependency>
***
### 文件说明	 
> `generatorConfig.xml` -> 主要配置文件，都是不变的配置   
> `generator-mysql.properties` -> 需要自定义的配置，被`generatorConfig.xml`文件引入

***