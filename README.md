MVNRepo
======================
This is a public Maven Repository hosted on GitHub that we use on [Mashape](http://www.mashape.com/). 

You are free to use in your projects, and contribute to it.

Usage
--------
Add the following code to your `pom.xml` for **releases** libraries:

``` xml
<repository>
	<id>mashape-releases</id>
	<url>https://github.com/Mashape/MVNRepo/raw/master/releases</url>
</repository>
```

Add the following code to your `pom.xml` for **snapshots** libraries:

``` xml
<repository>
	<id>mashape-snapshots</id>
	<url>https://github.com/Mashape/MVNRepo/raw/master/snapshots</url>
</repository>
```

How to contribute
--------
If you have a `*.jar` file, and you would like to distribute it in this Maven Repository, follow these steps:

1. Clone this GitHub repository
2. Execute the `mvn deploy:deploy-file` command:

```
mvn deploy:deploy-file -Dpackaging=jar \
  -DgroupId=GROUPID \
  -DartifactId=ARTIFACTID \
  -Dversion=VERSION \
  -Dfile=PATH-TO-FILE \
  -Durl=file:/path-to-MVNRepo/releases-or-snapshots
```

For example:

```
mvn deploy:deploy-file -Dpackaging=jar \
  -DgroupId=com.braintreegateway
  -DartifactId=braintree \
  -Dversion=2.13.1 \
  -Dfile=braintree-java-2.13.1.jar \
  -Durl=file:/path-to-MVNRepo/releases
```

or, if you want to preserve the original pom.xml

```
 mvn deploy:deploy-file -DpomFile=pom.xml -Dfile=PATH-TO-FILE -Durl=file:/path-to-MVNRepo/releases-or-snapshots
```
 
Be aware that the code above must be customized with the right arguments:

* `-DgroupId`
* `-DartifactId`
* `-Dversion`
* `-Dfile`
* `-Durl` (this could be `releases` or `snapshots`)

Releases
--------

###Braintree###
* Version: **2.13.2**
* Website: [http://www.braintreepayments.com](http://www.braintreepayments.com/)
  
``` xml
<dependency>
	<groupId>com.braintreegateway</groupId>
	<artifactId>braintree</artifactId>
	<version>2.13.2</version>
</dependency>
```

###Mashape File Manager###
* Version: **1.1.2**
* Website: [https://github.com/Mashape/file-manager](https://github.com/Mashape/file-manager)
  
``` xml
<dependency>
	<groupId>com.mashape.file-manager</groupId>
	<artifactId>mashape-file-manager</artifactId>
	<version>1.1.2</version>
</dependency>
```

###Mashape Java Client Library###
* Version: **1.3.2**
* Website: [https://github.com/Mashape/mashape-java-client-library](https://github.com/Mashape/mashape-java-client-library)

``` xml
<dependency>
	<groupId>com.mashape.clients</groupId>
	<artifactId>mashape-java-client</artifactId>
	<version>1.3.3</version>
</dependency>
```

###PDFCROWD###
* Version: **2.4**
* Website: [http://pdfcrowd.com/](http://pdfcrowd.com/)
  
``` xml
<dependency>
	<groupId>com.pdfcrowd</groupId>
	<artifactId>pdfcrowd</artifactId>
	<version>2.4</version>
</dependency>
```

###jbeandumer###
* Version: **1.5.1**
* Website: [http://code.google.com/p/jbeandumer/](http://code.google.com/p/jbeandumer/)

``` xml
<dependency>
	<groupId>ru.yandex.lc.jbd</groupId>
	<artifactId>jbeandumer</artifactId>
	<version>1.5.1</version>
</dependency>
```

###objectdumper###
* Version: **0.10**
* Website: [http://codevanrohde.nl/wordpress/?p=20](http://codevanrohde.nl/wordpress/?p=20)

``` xml
<dependency>
	<groupId>nu.rohde.objectdumper</groupId>
	<artifactId>objectdumper</artifactId>
	<version>0.10</version>
</dependency>
```


Snapshots
--------

###Morphia (MODIFIED VERSION, SEE URL)###
* Version: **1.0-appco**
* Website: [http://code.google.com/p/morphia/issues/detail?id=321](http://code.google.com/p/morphia/issues/detail?id=321)
  
``` xml
<dependency>
	<groupId>com.google.code.morphia</groupId>
	<artifactId>morphia</artifactId>
	<version>1.0-appco</version>
</dependency>
```

###Mongo Analyzer###
* Version: **1.0**
  
``` xml
<dependency>
	<groupId>com.mashape.mongo.analyzer</groupId>
	<artifactId>mongo-analyzer</artifactId>
	<version>1.0</version>
</dependency>
```
