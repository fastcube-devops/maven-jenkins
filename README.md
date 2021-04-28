# maven-jenkins
# project creation command :

  mvn archetype:generate  -DarchetypeGroupId=fr.fastconnect.factory.tibco.bw.maven -DarchetypeArtifactId=archetype-bw-default-project -DgroupId=com.fastcube.project -DartifactId=maven-jenkins -Dversion=1.0.0 -DbwProjectName=maven-jenkins -DrootProjectGroupId=fr.fastconnect.factory.tibco -DrootProjectArtifactId=fc-tibco-factory -DrootProjectVersidson=2.4.1 -DinteractiveMode=true
                        
# open the project with designer

  mvn bw:launch-designer
 
# package

  mvn package

# add/remove dependency

First we have to add the proj lib to the project 

mvn install:install-file -Dfile=C:\Users\Dev\Documents\repos\maven-jenkins\lib\LogLib.projlib -DgroupId=logging -DartifactId=logLib -Dversion=1.0.2 -Dtype=projlib -Dpackaging=projlib

Second we add the dependecy
mvn bw:<<add/remove>>-dependency -DdependencyGroupId=logging -DdependencyArtifactId=LogLib -DdependencyVersion=1.0.2 -DdependencyType=projlib -DdoIt=true
