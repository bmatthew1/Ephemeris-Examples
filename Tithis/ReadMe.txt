
javac -d . -cp libs\*;.; Tithis.java

java -cp libs\*;.; Tithis

copy con Manifest.txt
Main-Class: Tithis
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar -cvfm Tithis.jar Manifest.txt *.class libs

jar -tf Tithis.jar

java -jar Tithis.jar

javadoc -link https://docs.oracle.com/javase/8/docs/api/ -cp libs\*;.; -d docs *.java