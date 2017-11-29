# Java_JVM

Java ClassLoaders
 It dynamically loads the Java classes into JVM. So, Java Runtime Systems does not need to know the files or the file system to load java class.

#### There are 3 types of ClassLoaders
![ClassLoaders](https://2.bp.blogspot.com/-HCTsr-j_ojw/USTOh1f8JwI/AAAAAAAAAjg/YegPspR5K48/s400/java_classloader_hierarchy.PNG)
1.  Bootstrap class loader
*  It loads the core Java libraries located in the <JAVA_HOME>/jre/lib directory.
2.  Extensions class loader
* It loads the code in the extensions directories (<JAVA_HOME>/jre/lib/ext
3.  System class loader
* It loads code found on java.class.path


![ClassLoadersDetail](http://1.bp.blogspot.com/-0gOWex7Pb2E/USTOh2K7zpI/AAAAAAAAAjc/_viQADzxrsk/s1600/Java+classloader+working.PNG)

##  Java ClassLoader works in three principles
###  Delegation Principle
It forward the request to load class to parent classloader and it will only loaded if parent is not able to load the class.
###  Visibility Principle
Child ClassLoader are allowed to see class loaded by Parent ClassLoader but vice-versa is not true.

###  Uniqueness Principle
It says that class loaded by Parent should not be loaded by Child ClassLoader again. In other words, It allows to load a class exactly once
