Easy but not secure way
```java
System.getProperty('user.name')
```
`java -Duser.name=SLF` can hack it

Better way
For \*nix

```
new UnixSystem().getName()
```

For windows
```java
new NTSystem().getName()
```

One more thing, `UnixSystem` and `NTSystem` can get other infomation about the system
