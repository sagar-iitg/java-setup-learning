```
 C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\javac.exe  HellWorld.java
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\java.exe  HelloWorld
```

```
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\javac.exe  pkg/CharactertoInteger.java



C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\java.exe  pkg/CharactertoInteger
C:\'Program Files'\'Eclipse Adoptium'\jdk-17.0.6.10-hotspot\bin\java.exe  pkg.CharactertoInteger
```
### In Poweshell
```
PS C:\Users\ksaga\OneDrive\Desktop\New folder> & "C:\Program Files\Eclipse Adoptium\jdk-17.0.6.10-hotspot\bin\javac.exe" .\pkg\CharactertoInteger.java

 & "C:\Program Files\Eclipse Adoptium\jdk-17.0.6.10-hotspot\bin\java.exe" pkg.CharactertoInteger
 
 & "C:\Program Files\Eclipse Adoptium\jdk-17.0.6.10-hotspot\bin\java.exe" pkg/CharactertoInteger
```

###
& is not needed for cmd

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









```
Use Target Version: When compiling your code using Java 17, you can use the -target option to specify that you're targeting Java 8 bytecode. This ensures that the generated bytecode is compatible with Java 8, but it doesn't prevent you from using Java 17 language features. So, you need to be very cautious when using this approach and avoid using any Java 17-specific features in your code.

javac -source 17 -target 8 YourSourceFile.java


In summary, running Java 8 compiled code on Java 17 can work, but it's essential to test thoroughly and be aware of potential compatibility issues. Keeping your code up to date with the latest Java versions is generally a good practice to ensure you can take advantage of new features and security enhancements.

```



```

javac -source 7 -target 8 YourSourceFile.java

Yes, it is possible to use javac with -source 7 and -target 8 options to compile Java code written with Java 7 language features (source compatibility) and generate bytecode that targets Java 8 (bytecode compatibility). This approach allows you to write code using Java 7 features and then run it on a Java 8 runtime environment.



javac -source 8 -target 7 YourSourceFile.java

this is not possible
```
