在mac下使用
```
echo ${JAVA_HOME}
```
是看不到`JAVA_HOME`的设置的。

使用`env`命令也看不到JAVA_HOME的值。

解决方法`/usr/libexec/java_home -V`:
```
$ /usr/libexec/java_home -V
Matching Java Virtual Machines (1):
    1.8.0_66, x86_64:	"Java SE 8"	/Library/Java/JavaVirtualMachines/jdk1.8.0_66.jdk/Contents/Home

/Library/Java/JavaVirtualMachines/jdk1.8.0_66.jdk/Contents/Home
```

