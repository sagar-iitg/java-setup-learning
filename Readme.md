```
 C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\javac.exe  HellWorld.java
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\java.exe  HelloWorld
```

```
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\javac.exe  pkg/CharactertoInteger.java
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\java.exe  pkg/CharactertoInteger
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\java.exe  pkg.CharactertoInteger
```


```
The key takeaway is that you specify the source file with the relative path
 to the package structure during compilation (mypackage/MyPackageExample.java),
but you use the fully qualified class name during execution (mypackage.MyPackageExample).
This ensures that the Java compiler correctly identifies the package and compiles the code accordingly.
```

```
Classfile Format: Check the major and minor version numbers in the class file header.
The major version indicates the Java version,
and the minor version may provide additional details.
Here's a mapping of major version numbers to Java versions:

52: Java 8
53: Java 9
54: Java 10
55: Java 11
56: Java 12
57: Java 13
58: Java 14
59: Java 15
60: Java 16
61: Java 17 (as of my knowledge cutoff in September 2021)
You can use tools like javap (included with the JDK) to inspect the classfile format:

```


```
javap -verbose YourClass.class | findstr "major"
 javap -verbose CharactertoInteger.class | findstr "major"
```
