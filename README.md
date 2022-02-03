# maven-project

**maven commands**

1. mvn clean
This command cleans the maven project by deleting the target directory. The command output relevant messages are shown below.
$ mvn clean

2. mvn compiler:compile
This command compiles the java source classes of the maven project.
$ mvn compiler:compile

3. mvn compiler:testCompile
This command compiles the test classes of the maven project.
$ mvn compiler:testCompile

4. mvn package
This command builds the maven project and packages them into a JAR, WAR, etc.
$ mvn package

The output shows the location of the JAR file just before the “BUILD SUCCESS” message. Notice the package goal executes compile, testCompile, and test goals before packaging the build.

5. mvn install
This command builds the maven project and installs the project files (JAR, WAR, pom.xml, etc) to the local repository.

6. mvn deploy
This command is used to deploy the artifact to the remote repository. The remote repository should be configured properly in the project pom.xml file distributionManagement tag. The server entries in the maven settings.xml file is used to provide authentication details.

7. mvn validate
This command validates the maven project that everything is correct and all the necessary information is available.

8. mvn dependency:tree
This command generates the dependency tree of the maven project.
$ mvn dependency:tree

9. mvn dependency:analyze
This command analyzes the maven project to identify the unused declared and used undeclared dependencies. It’s useful in reducing the build size by identifying the unused dependencies and then remove it from the pom.xml file.
$ mvn dependency:analyze

10. mvn archetype:generate
Maven archetypes is a maven project templating toolkit. We can use this command to generate a skeleton maven project of different types, such as JAR, web application, maven site, etc.

11. mvn site:site
This command generates a site for the project. You will notice a “site” directory in the target after executing this command. There will be multiple HTML files inside the site directory that provides information related to tMaven site Command

12. mvn test
This command is used to run the test cases of the project using the maven-surefire-plugin.
$ mvn test

13. mvn compile
It’s used to compile the source Java classes of the project.
$ mvn compile

14. mvn verify
This command build the project, runs all the test cases and run any checks on the results of the integration tests to ensure quality criteria are met.


