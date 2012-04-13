MVNRepo
======================
This is a public Maven Repository hosted on GitHub that we use on [Mashape](http://www.mashape.com/). 

You are free to use in your projects, and contribute to it.

Usage
--------
Add the following code to your `pom.xml` for **releases** libraries:

``` xml
<repository>
	<id>thefosk-releases</id>
	<url>https://github.com/thefosk/MVNRepo/raw/master/releases</url>
</repository>
```

Add the following code to your `pom.xml` for **snapshots** libraries:

``` xml
<repository>
	<id>thefosk-snapshots</id>
	<url>https://github.com/thefosk/MVNRepo/raw/master/snapshots</url>
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
* Version: **1.0**
* Website: [https://github.com/Mashape/file-manager](https://github.com/Mashape/file-manager)
  
``` xml
<dependency>
	<groupId>com.mashape.file-manager</groupId>
	<artifactId>mashape-file-manager</artifactId>
	<version>1.0</version>
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
