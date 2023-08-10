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
