# WildFly Docker image

This is an example Dockerfile with [WildFly application server](http://wildfly.org/).

## Usage

To boot in standalone mode

    docker run -it jboss/wildfly
    
To boot in standalone mode with admin console available remotely

    docker run -p 8080:8080 -p 9990:9990 -it jboss/wildfly /opt/jboss/wildfly/bin/standalone.sh -b 0.0.0.0 -bmanagement 0.0.0.0
    
## Java version

In contrast to [official git repository](https://github.com/jboss-dockerfiles/wildfly) 
this image is based on Java 8