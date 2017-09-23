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
    <groupId>com.oracle.jdbc</groupId>
    <artifactId>ojdbc8</artifactId>
    <version>12.2.0.1</version>
</dependency>
```


#### 11.2.0.4

```
mvn install:install-file -Dfile=lib/jdbc/ojdbc6.jar -Dpackaging=jar -DgroupId=com.oracle.jdbc -DartifactId=ojdbc6 -Dversion=11.2.0.4
```

```xml
<dependency>
    <groupId>com.oracle.jdbc</groupId>
    <artifactId>ojdbc6</artifactId>
    <version>11.2.0.4</version>
</dependency>
```

### MS SQL

### DB2

## IBM MQ

 - [Installation and configuration of IBM MQ classes for Java](https://www.ibm.com/support/knowledgecenter/en/SSFKSJ_8.0.0/com.ibm.mq.dev.doc/q030580_.htm)
 - [What is installed for IBM MQ classes for Java](https://www.ibm.com/support/knowledgecenter/en/SSFKSJ_8.0.0/com.ibm.mq.dev.doc/q030590_.htm)

```
mvn install:install-file -Dfile=lib/mq/com.ibm.mq.allclient.jar -Dpackaging=jar -DgroupId=com.ibm.mq -DartifactId=com.ibm.mq -Dversion=8.0.x
mvn install:install-file -Dfile=lib/mq/com.ibm.mqjms.jar -Dpackaging=jar -DgroupId=com.ibm.mq -DartifactId=com.ibm.mqjms -Dversion=8.0.x
```
```xml
<dependency>
    <groupId>com.ibm.mq</groupId>
    <artifactId>com.ibm.mq</artifactId>
    <version>8.0.x</version>
</dependency>
<dependency>
    <groupId>com.ibm.mqjms</groupId>
    <artifactId>com.ibm.mqjms</artifactId>
    <version>8.0.x</version>
</dependency>
```

```xml
<repositories>
    <repository>
        <id>3rd-party-repo</id>
        <name>3rd party repo</name>
        <url>https://junlapong.github.com/mvn</url>
    </repository>
</repositories>
```

