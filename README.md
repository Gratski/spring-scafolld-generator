# spring-scafolld-generator
## What is going to be generated under your C:\workspace\
### A Maven project with the following data structure:
- <folderName>
  - <groupId>.parent/
    - <groupId>.persistence/
    - <groupId>.business/
    - <groupId>.dto/
    - <groupId>.rest/
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
### Unzip the content
### Run: java com.voxel.generator.spring.v1.jar SpringProjectGenerator <folderName> <groupId>
### Build: mvn install
  
