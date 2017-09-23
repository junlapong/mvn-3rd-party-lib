Maven 3rd Party
===============

Install 3rd party library to maven local repository

```
git clone https://github.com/junlapong/mvn-3rd-party-lib.git

cd mvn-3rd-party-lib
```

## JDBC Driver

### Oracle

#### 12.2.0.1

```
mvn install:install-file -Dfile=lib/jdbc/ojdbc8.jar -Dpackaging=jar -DgroupId=com.oracle.jdbc -DartifactId=ojdbc8 -Dversion=12.2.0.1
```

```xml
<dependency>
    <groupid>com.oracle.jdbc</groupid>
    <artifactid>ojdbc8</artifactid>
    <version>12.2.0.1</version>
</dependency>
```


#### 11.2.0.4

```
mvn install:install-file -Dfile=lib/jdbc/ojdbc6.jar -Dpackaging=jar -DgroupId=com.oracle.jdbc -DartifactId=ojdbc6 -Dversion=11.2.0.4
```

```xml
<dependency>
    <groupid>com.oracle.jdbc</groupid>
    <artifactid>ojdbc6</artifactid>
    <version>11.2.0.4</version>
</dependency>
```

### MS SQL

### DB2

## IBM MQ

 - [Installation and configuration of IBM MQ classes for Java](https://www.ibm.com/support/knowledgecenter/en/SSFKSJ_8.0.0/com.ibm.mq.dev.doc/q030580_.htm)
 - [What is installed for IBM MQ classes for Java](https://www.ibm.com/support/knowledgecenter/en/SSFKSJ_8.0.0/com.ibm.mq.dev.doc/q030590_.htm)

```xml
<repositories>
    <repository>
        <id>3rd-party-repo</id>
        <name>3rd party repo</name>
        <url>https://junlapong.github.com/mvn</url>
    </repository>
</repositories>
```

