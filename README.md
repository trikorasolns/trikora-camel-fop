# trikora-camel-fop
Apache Camel FOP (2.1) feature for OSGi Bundle Repository (OBR)

This project enables a new feature for installing Apache FOP 2.1 in Apache Servicemix. Each feature file relates to a Apache Servicemix version. There are 2 versions of the feature, _a_ and _b_. _a_ is the default _camel-fop_ feature  and _b_ installs Apache FOP 2.1.

## Installation guide
1. Download the corresponding feature file to a folder named _feature-repository_ in your Apache Servicemix folder.
2. Open the Apacher Servicemix Console
3. Add the feature file to 
```sh
karaf@root>feature:addUrl file:feature-repository/trikora-fop-2.14.3-features.xml
```
4. Install the FOP 2.1 feature
```sh
karaf@root>feature:install trikora-fop/2.14.3_b
```
Apache FOP will be installed.

## Known issues
Installing this feature won't enable any of the following:
* FopComponents
* FopEndpoint
* FopConsumer

-------
This project is provided by [Trikora Solutions](http://www.trikorasolutions.com/).