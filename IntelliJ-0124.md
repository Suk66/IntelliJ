**화이팅**

# Spring-context값 안 먹는 부분. 
- 우측 Maven선택후 Reload
- cmd 창 가서 해당 프로젝트 폴더로 이동후
-  D: cd D:\ncs\workspace(intelliJ)\orderSystem
-  mvn clean install -u 입력.
```java
<dependency>
      <groupId>org.springframework</groupId>
      <artifactId>spring-context</artifactId>
      <version>6.0.2</version>
    </dependency>
```


```java
<dependency>
    <groupId>org.springframework</groupId>
    <artifactId>spring-context</artifactId>
    <version>6.0.2</version> <!-- Spring 버전에 맞는 값을 사용 -->
</dependency>
```


**beans config**
#Applicationcontext 사용시(?)
```java
<?xml version="1.0" encoding="UTF-8"?>
<beans xmlns="http://www.springframework.org/schema/beans"
       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
       xsi:schemaLocation="http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans.xsd">
</beans>
```
