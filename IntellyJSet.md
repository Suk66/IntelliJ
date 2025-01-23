***💎💎💎서로 다른 JDK를 사용하는 IDE를 옮겨 다닐 때 bat파일을 만들어서 쉽게 적용 하는 방법💎💎💎***
#윈도우기준.
-jdk17 active
@echo off
set JAVA_HOME=C:\Program Files\Java\jdk-17
set PATH=%JAVA_HOME%\bin;%PATH%
echo Switched to Java 17
cmd

-jdk11 active
@echo off
set JAVA_HOME=C:\Program Files\Java\jdk-11
set PATH=%JAVA_HOME%\bin;%PATH%
echo Switched to Java 11
cmd
