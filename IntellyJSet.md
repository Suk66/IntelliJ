***💎💎💎서로 다른 JDK를 사용하는 IDE를 옮겨 다닐 때 bat파일을 만들어서 쉽게 적용 하는 방법💎💎💎***

#윈도우기준

**강조**

```java
jdk17 active
@echo off*
set JAVA_HOME=C:\Program Files\Java\jdk-17
set PATH=%JAVA_HOME%\bin;%PATH%
echo Switched to Java 17
echo JAVA_HOME: %JAVA_HOME%
start "" "C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2024.3.2\bin\idea64.exe"
exit
```

```cmd
-jdk11 active
@echo off
set JAVA_HOME=C:\Program Files\Java\jdk-11
set PATH=%JAVA_HOME%\bin;%PATH%
echo Switched to Java 11
echo JAVA_HOME: %JAVA_HOME%
start "" "C:\Program Files\SpringToolSuite4\STS.exe"
exit
```

**DATA**
 - getter
 - setter
 - tostring
 - instructor
 - -????


**lombok**
#코드다이어터

```java
<!-- https://mvnrepository.com/artifact/org.projectlombok/lombok -->
    <dependency>
      <groupId>org.projectlombok</groupId>
      <artifactId>lombok</artifactId>
      <version>1.18.36</version>
      <scope>provided</scope>
    </dependency>
```





**Log**
#@Slf4j
- 버전인식을 못해서 위에 있는 jdk17 bat파일을 만들어서 직접 강제로 IntelliJ로 접속해서 Jdk17을 지정하게 모든 셋팅을 맞췄음.
- 인텔리제이는.. JDK17을 인식하지만 문제는 MAVEN(내장)이  윈도우 환경변수 설정에 JDK11을 계속 지정하는 문제 발생.
- 허나 STS를 사용할 때 JDK11을 지정해야 하기 때문에 환경 변수 값은 건들지 않고 있음.
- IntelliJ설정과 MAVEN설정으로 주도 함.
- 추가로 레벨로그가 초과하면 로그가 안 뜨는데 그문제는 다른 방식으로 또 해결해야 함.

```java
<!-- SLF4J API (필수) -->
    <dependency>
      <groupId>org.slf4j</groupId>
      <artifactId>slf4j-api</artifactId>
      <version>2.0.13</version>
    </dependency>

    <!-- SLF4J 구현체: slf4j-simple (간단한 로그 출력) -->
    <dependency>
      <groupId>org.slf4j</groupId>
      <artifactId>slf4j-simple</artifactId>
      <version>2.0.13</version>
    </dependency>
```





