This project is a java portage of [geomodel python project](http://code.google.com/p/geomodel/). Have a look at it to get more information about geocells algorithm.

## How to use java geomodel ##

  1. Get the jar:
  * If you use maven, install [svn wagon](http://maven-svn-wagon.googlecode.com/svn/site/index.html) and then in your pom.xml declare a repository:
> > `

&lt;repository&gt;


> > > 

&lt;id&gt;

javageomodel-repo

&lt;/id&gt;


> > > 

&lt;name&gt;

GeocellJava Repository

&lt;/name&gt;


> > > 

&lt;url&gt;

http://javageomodel.googlecode.com/svn/repository

&lt;/url&gt;


> > > 

&lt;/repository&gt;


> > > `
and add the dependency:

> > `

&lt;dependency&gt;


> > > 

&lt;groupId&gt;

com.beoui

&lt;/groupId&gt;


> > > 

&lt;artifactId&gt;

geocell

&lt;/artifactId&gt;


> > > 

&lt;version&gt;

0.0.4 **check the last version available on the repository**

&lt;/version&gt;



> > 

&lt;/dependency&gt;

`
  * If you don't use maven, download the latest jar: [maven repo](http://code.google.com/p/javageomodel/source/browse/#svn/repository/com/beoui/geocell)
**The download of [geomodel.jar](http://code.google.com/p/javageomodel/downloads/list) is DEPRECATED.**
  1. Use method GeocellManager.generateGeoCell to get geocell list and save them in your entity
  1. Use method GeocellManager.bestBboxSearchCells to get optimized geocell list to be used in bounding box query.
  1. Use method GeocellManager.proximityFetch to search for entities following proximity fetch algorithm.

More information and example in the test class [HowToUseGeocell](http://code.google.com/p/javageomodel/source/browse/trunk/geocell/src/test/java/com/beoui/utils/HowToUseGeocell.java) and in javadoc.

Check the pom.xml for all jar dependencies.

## JDO/JPA compatibility ##

Thanks to the awesome work of Ricardo Gladwell, the library is now compatible with JPA (and library is more tested and cleaner too thanks to him =) )...

## Any Questions? ##

Please ask question on the google group [javageomodel-discuss](http://groups.google.com/group/javageomodel-discuss).