
javac -d . -cp libs\swisseph-2.01.00-01.jar;.; VedicHouses.java

java -cp libs\swisseph-2.01.00-01.jar;.; VedicHouses

copy con Manifest.txt
Main-Class: VedicHouses
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar cvfm VedicHouses.jar Manifest.txt *.class libs ephe

jar tf VedicHouses.jar

java -jar VedicHouses.jar