# Intro-to-Ant
Examples of basic tasks (directory creation, file creation, copying, deleting directory contents and accessing environment variables) using ANT

**Commands to perform the basic tasks in ANT** <br/>
1.To create a directory:<br/>
```xml
<mkdir dir="dir-name" />
```
2.To create a file in already created directory:<br/>
```xml
<touch file="dir-name/file-name.extension">
</touch>
```
3.To print a message<br/>
```xml
<echo>Message included here...</echo>
```
4. Create property to access environment variable in build file<br/>
```xml
<property environment="env" />
<property name="JAVA_HOME" value="${env.JAVA_HOME}" />
```
5. Copying file from one directory to another
```xml
<copy file="path-to-file(source)/file-name.extension" todir="path-to-destination" />
```
6. Deleting a file
```xml
<delete file="path-to-file/file-name.extension" />
```
7. Deleting a directory
```xml
<delete dir="Hello-World" />
```
