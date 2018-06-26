
javac -d . -cp libs\swisseph-2.01.00-01.jar;.; Tithis.java

java -cp libs\swisseph-2.01.00-01.jar;.; Tithis

copy con Manifest.txt
Main-Class: Tithis
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar cvfm Tithis.jar Manifest.txt *.class libs

jar tf Tithis.jar

java -jar Tithis.jar

javadoc -link http://www.th-mack.de/download/swisseph-doc/ -link https://docs.oracle.com/javase/8/docs/api/ -cp libs\swisseph-2.01.00-01.jar;.; -d docs *.java