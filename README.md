# CI-JaCoCo-Jenkins

Steps to implement continous integration with Maven project and JaCoCo in Jenkins-

```

1. Add the JaCoCo plugin in Jenkins under manage Jenkins-

2. Create a Maven project in terminal-
$ mvn archetype:generate -DgroupId=CodeCoverageDemo -DartifactId=MathOperations -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

3. Navigate to the maven project as shown below:
$ cd /home/labsuser/MathOperations
$ vi pom.xml

4. Delete the existing code in the pom.xml file and add the code in this Github repository.

5. Create a simple Java application after removing existing Java file-
$ cd /home/labsuser/MathOperations/src/main/java/CodeCoverageDemo
$ rm App.java
$ vi Operations.java 
Add the code in this Github repo.

6. Add the test Java file after replacing the existing file-
$ cd /home/labsuser/MathOperations/src/test/java/CodeCoverageDemo
$ rm AppTest.java
$ vi OperationsTest.java 
Add the code in this Github repo.

7. Create a Maven Jenkins Job and in the Build section of your job, for Root POM give the path of the pom.xml in your local system as shown below:
/home/labsuser/MathOperations/pom.xml

8. Build the Job and view the console output.

```

