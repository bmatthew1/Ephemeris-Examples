
javac -encoding utf8 -d . -cp libs\*;.; NakshatraDates.java

java -cp libs\*;.; NakshatraDates

copy con Manifest.txt
Main-Class: NakshatraDates
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar -cvfm NakshatraDates.jar Manifest.txt *.class libs

jar -tf NakshatraDates.jar

java -jar NakshatraDates.jar

javadoc -encoding utf8 -link https://docs.oracle.com/javase/8/docs/api/ -cp libs\*;.; -d docs *.java