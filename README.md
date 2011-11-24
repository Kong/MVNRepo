MVNRepo
======================
This is a public Maven Repository hosted on GitHub that we use on Mashape. 

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

Releases
--------

###Braintree###
* Version: **2.13.1**
* Website: [http://www.braintreepayments.com](http://www.braintreepayments.com/)
  
``` xml
<dependency>
	<groupId>com.braintreegateway</groupId>
	<artifactId>braintree</artifactId>
	<version>2.13.1</version>
</dependency>
```