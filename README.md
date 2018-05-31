# springFramework

## run spring(maven)
### maven batch script
```
mvn install && cp -rf target/*.war $CATALINA_HOME/webapps/${current.project.name}.war && java -Djdk.tls.ephemeralDHKeySize=2048 -classpath $CATALINA_HOME/bin/bootstrap.jar:$CATALINA_HOME/bin/tomcat-juli.jar -Dcatalina.base=$CATALINA_HOME -Dcatalina.home=$CATALINA_HOME -Djava.io.tmpdir=$CATALINA_HOME/temp org.apache.catalina.startup.Bootstrap start
```
