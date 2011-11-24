MVNRepo
======================
This is a public MVN repository hosted on GitHub. You're free to use it in your projects and contribute with new libraries.

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

Releases
--------

###Braintree###
* ([braintreepayments.com](http://www.braintreepayments.com/))
* Version **2.13.1**
  
``` xml
<dependency>
	<groupId>com.braintreegateway</groupId>
	<artifactId>braintree</artifactId>
	<version>2.13.1</version>
</dependency>
```