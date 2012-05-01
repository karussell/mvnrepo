### My micro maven repo

## A Java readability clone (extracts important text and image) at https://github.com/karussell/snacktory
<dependency>
     <groupId>de.jetwick</groupId>
     <artifactId>snacktory</artifactId>
     <version>1.1-SNAPSHOT</version>
</dependency>

## An example war at https://github.com/karussell/ElasticSearchExample

## The plotter at https://github.com/karussell/plotter
<dependency>
     <groupId>de.genvlin</groupId>
     <artifactId>plotter</artifactId>
     <version>1.0-SNAPSHOT</version>
</dependency>

## A twitter utility
<dependency>
     <groupId>de.jetsli</groupId>
     <artifactId>twittertool</artifactId>
     <version>1.0-SNAPSHOT</version>
</dependency>


## USAGE

<repository>
  <id>karussell_snapshots</id>
  <url>https://github.com/karussell/mvnrepo/raw/master/snapshots/</url>
</repository>             

<repository>
  <id>karussell_releases</id>           
  <url>https://github.com/karussell/mvnrepo/raw/master/releases/</url>                   
</repository> 

## If you want to do the same read:
http://cemerick.com/2010/08/24/hosting-maven-repos-on-github/

Hint add a distributionManagement tag in the pom.xml and do
mvn -DaltDeploymentRepository=snapshot-repo::default::file:/path/to/mvnrepo/snapshots/ clean deploy -Dmaven.test.skip=true