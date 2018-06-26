
javac -d . -cp libs\swisseph-2.01.00-01.jar;.; AriesRising.java

java -cp libs\swisseph-2.01.00-01.jar;.; AriesRising

copy con Manifest.txt
Main-Class: AriesRising
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar cvfm AriesRising.jar Manifest.txt *.class libs

jar tf AriesRising.jar

java -jar AriesRising.jar