# Spring Basic MVC project structure generator

This jar allows you to create a maven based java spring project without having to do the basic configuration of the 4 more usual projects:
- Persistence Project
- Business Project
- Data Transfer Objects Project
- REST API Project

This creates the strucuture ready to be built with maven, but they have no logic associated and no cross module dependency.
To do that you just have to add the module as a dependency, as you would do in a regular maven multi-module project.

### What is going to be generated under your C:\workspace\
#### A Maven project with the following data structure:
- FOLDER_NAME
  - GROUP_ID.parent/
    - GROUP_ID.persistence/
    - GROUP_ID.business/
    - GROUP_ID.dto/
    - GROUP_ID.rest/
    - pom.xml
  
Each folder under <groupId>.parent is a module and it has the following data structure:
  - src/
    - main/
      - java/
      - resources/
    - test/
      - java
      - resources
  - pom.xml

## To run the generator
Download the .jar file

Run: java -cp com.voxel.generator.spring-v1.jar com.voxel.generator.spring.SpringProjectGenerator FOLDER_NAME MAVEN_GROUP_ID

Build: mvn install
