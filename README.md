# maven-jenkins
# project creation command :

  mvn archetype:generate  -DarchetypeGroupId=fr.fastconnect.factory.tibco.bw.maven 
                          -DarchetypeArtifactId=archetype-bw-default-project 
                          -DgroupId=com.fastcube.project 
                          -DartifactId=maven-jenkins 
                          -Dversion=1.0.0 
                          -DbwProjectName=maven-jenkins 
                          -DrootProjectGroupId=fr.fastconnect.factory.tibco 
                          -DrootProjectArtifactId=fc-tibco-factory 
                          -DrootProjectVersidson=2.4.1 
                          -DinteractiveMode=true
                        
# open the project with designer

  mvn bw:launch-designer
 
# package

  mvn package
