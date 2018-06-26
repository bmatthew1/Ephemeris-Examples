
JAVA_TOOL_OPTIONS: -Dfile.encoding=UTF8

javac -d . -cp libs\swisseph-2.01.00-01.jar;.; NakshatraDates.java

java -cp libs\swisseph-2.01.00-01.jar;.; NakshatraDates

copy con Manifest.txt
Main-Class: NakshatraDates
Class-Path: libs\swisseph-2.01.00-01.jar
^Z

jar cvfm NakshatraDates.jar Manifest.txt *.class libs

jar tf NakshatraDates.jar

java -jar NakshatraDates.jar

javadoc -link http://www.th-mack.de/download/swisseph-doc/ -link https://docs.oracle.com/javase/8/docs/api/ -cp libs\swisseph-2.01.00-01.jar;.; -d docs *.java