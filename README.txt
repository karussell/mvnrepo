My micro maven repo for the projects at

https://github.com/karussell/snacktory
<dependency>
     <groupId>de.jetwick</groupId>
     <artifactId>snacktory</artifactId>
     <version>1.0-SNAPSHOT</version>
</dependency>

( and the example war at https://github.com/karussell/ElasticSearchExample)


to include the repository use

<repository>
  <id>karussell_snapshots</id>
  <url>https://github.com/karussell/mvnrepo/raw/master/snapshots/</url>
</repository>             

<repository>
  <id>karussell_releases</id>           
  <url>https://github.com/karussell/mvnrepo/raw/master/releases/</url>                   
</repository> 

If you want to do the same read:
http://cemerick.com/2010/08/24/hosting-maven-repos-on-github/

hint:
mvn -DaltDeploymentRepository=snapshot-repo::default::file:/path/to/mvnrepo/snapshots/ clean deploy -Dmaven.test.skip=true