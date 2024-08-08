 This page shall describe the steps needed to manipulate the java-maven-dummy for test-cases and show-cases

 # Preparation
You merely need an editor.

# Add a "fake" dependency
1. Create a test- or demo-branch acc. to the guidance in ../Tooling-Landscape/Dummy_Repositories/README.md
2. Select a dependency in https://mvnrepository.com/
3. Open the editor for the respective pom-file in the branch
4. add the new dependency coordinate in the pom-file <dependencies>-section e.g. 
    <dependency>
        <groupId>org.apache.logging.log4j</groupId>
        <artifactId>log4j</artifactId>
        <version>2.14.0</version>
        <type>pom</type>
    </dependency>
5. save the file
6. commit your changes
7. push the changes to the repository
8. run a test with a SCA-tooling of your choice to check if the new dependency had to expected effect
9. document the testcase/democase in the respective doc/... branch including the expected result


