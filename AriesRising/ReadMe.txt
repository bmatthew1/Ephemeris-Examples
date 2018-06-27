
javac -d . -cp libs\*;.; AriesRising.java

java -cp libs\*;.; AriesRising

copy con Manifest.txt
Main-Class: AriesRising
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar -cvfm AriesRising.jar Manifest.txt *.class libs

jar -tf AriesRising.jar

java -jar AriesRising.jar

javadoc -link https://docs.oracle.com/javase/8/docs/api/ -cp libs\*;.; -d docs *.java