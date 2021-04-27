# SocialNetworkingApp
## Students: Adjudeanu Patrik, Ionescu Matei

The purpose of this project is creating an application that helps students talk to eachother, and find groups matching their interests.

#### Implementation
Build Tool: Gradle  
Language: Java (JavaFX as GUI library) 
DBMS: H2 (thanks to its Java compatibility)  


#####H2 installation
- Download H2 by following the instructions given on their offigial website(http://www.h2database.com/html/quickstart.html)
- Declare H2 in plugins section of the build file(id "edu.umich.med.michr.h2-plugin" version "0.1.1-SNAPSHOT")
- Declare H2 as a testing, runtime and compilation dependency:

  (testCompile group: 'com.h2database', name: 'h2', version: '1.4.200'
  runtime 'com.h2database:h2:1.4.200'
  compile group: 'com.h2database', name: 'h2', version: '1.4.200')
- Log in with:

  path: jdbc:h2:tcp://localhost/~/test
  user: sa(no password)

- Import database(export file is database.txt)