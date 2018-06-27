
javac -d . -cp libs\*;.; VedicHouses.java

java -cp libs\*;.; VedicHouses

copy con Manifest.txt
Main-Class: VedicHouses
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar -cvfm VedicHouses.jar Manifest.txt *.class libs ephe

jar -tf VedicHouses.jar

java -jar VedicHouses.jar

javadoc -link https://docs.oracle.com/javase/8/docs/api/ -cp libs\*;.; -d docs *.java