Software & Dependencies
IntelliJ Community Edition Version 2021.3.2
JDK Version 17.0.2
Apache Maven
Note: This dependency can be imported using IntelliJ.
Go to "File" > "New Project" and then selecting "Maven" as the project structure.
JUnit Jupiter API Version 5.8.2
Note: This dependency can be imported within Intellij using Apache Maven and IntelliJ's built-in dependency generator.
Alternatively you can open the Maven "pom.xml" file and paste in the following code within the "dependencies" section of the file:
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter</artifactId>
        <version>5.8.2</version>
    </dependency>
JUnit Vintage Engine Version 5.6.1
Note: This dependency can be imported within Intellij using Apache Maven and IntelliJ's built-in dependency generator.
Alternatively you can open the Maven "pom.xml" file and paste in the following code within the "dependencies" section of the file:
   <dependency>
        <groupId>org.junit.vintage</groupId>
        <artifactId>junit-vintage-engine</artifactId>
        <version>5.6.1</version>
        <scope>test</scope>
    </dependency>
Selenium Java Version 4.1.2
Note: This dependency can be imported within Intellij using Apache Maven and IntelliJ's built-in dependency generator.
Alternatively you can open the Maven "pom.xml" file and paste in the following code within the "dependencies" section of the file:
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>4.1.2</version>
    </dependency> 
Cucumber JVM: Java Version 7.2.3
Note: This dependency can be imported within Intellij using Apache Maven and IntelliJ's built-in dependency generator.
Alternatively you can open the Maven "pom.xml" file and paste in the following code within the "dependencies" section of the file:
    <dependency>
        <groupId>io.cucumber</groupId>
        <artifactId>cucumber-java</artifactId>
        <version>7.2.3</version>
    </dependency> 
Cucumber JVM: JUnit Version 7.2.3
Note: This dependency can be imported within Intellij using Apache Maven and IntelliJ's built-in dependency generator.
Alternatively you can open the Maven "pom.xml" file and paste in the following code within the "dependencies" section of the file:
    <dependency>
        <groupId>io.cucumber</groupId>
        <artifactId>cucumber-junit</artifactId>
        <version>7.2.3</version>
    </dependency>

↥ back to top

How to use
Navigate to the top of this GitHub repo and click the green Code button. This will open a menu where you will want to click Download Zip.


Having clicked Download ZIP a Show In Folder dialogue box will open. Choose where you want to store the compressed Sauce Demo Framework program and then click the Save button.


Using Windows Explorer navigate to the location you saved the compressed Sauce Demo Framework program in. Right-click on the program and select Extract All.


Open IntelliJ Community Edition and click File and then Open. Navigate to the extracted Sauce Demo Framework program project folder and select it. Then click Ok.


This project doesn't include the Web Drivers for the different browsers, so, you must download and place them into the right folder. The standard folder path used for this project is src/test/resources/{webDriver_file_name}". In this example is shown ChromeDriver.exe as web driver used.


Once the project has opened and all dependencies have been downloaded you must run the TestRunner file. This file should be in src/test/java/org/runewriters/stepdefs. This will allow you to run all features files in one go. You can now run the program by clicking the green play button.



↥ back to top

Project Scope
The framework worked under the Project Object Model, which provides all the configuration for a single project:

POM: Classes that represent the methods with different behaviours in each web page.
Step Defs: The actual tests based in BDD. This is backside of the user stories.
Web Drivers: Drivers that allows you to test the feature files in different browsers.
Feature Files: Files that represent the user stories adapted to BDD. Each scenario represents an user behaviour on the website through different web pages.
