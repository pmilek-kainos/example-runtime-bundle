# example-runtime-bundle

Example Runtime Bundle
This repository contains an Example Runtime Bundle used by the Activiti Cloud Examples.

1. export myapp.zip from modeling or `cd src/main/resources && zip -r myapp.zip processes/* && rm -rf processes/`
2. install in local maven repo via `mvn install:install-file -Dfile=myapp.zip -DgroupId=org.activiti.cloud.examples -DartifactId=myapp -Dversion=1.0 -Dpackaging=jar`
3. delete file `rm myapp.zip`
4. add maven-dependency-plugin config to pom.xml bound to generate-resources phase  