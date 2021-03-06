# Java EE 7 - Angular - Sample Application #

Original code taken from [https://github.com/radcortez/javaee7-angular](https://github.com/radcortez/javaee7-angular)

## Blog posts ##

* [Java EE 7 with Angular JS – Part 1](http://www.radcortez.com/java-ee-7-with-angular-js-part-1)

* [Java EE 7 with Angular JS – CRUD, REST, Validations – Part 2](http://www.radcortez.com/java-ee-7-with-angular-js-crud-rest-validations-part-2)


## How to run ? ##

## Localhost ##

* You need JDK 8 or higher, Maven 3 and Wildfly 8 or Glassfish 4.1 to run the application.
* Build the code using Maven with the command: `mvn clean install`.

### Deploy in Wildfly 10 ###

  * Copy the file javaee7-angular.war from target directory to your Wildfly installation folder
  `standalone/deployments`

  * You can also deploy the app using the Maven Wildfly Plugin with the following command: `mvn wildfly:deploy`. You need to have Wildfly running.

  * Start Wildfly and go to http://localhost:8080/javaee7-angular/ (http://localhost:8080/javaee7-angular/)
  
### Deploy in Embedded Wilffy ###

  * Just run `mvn wildfly:run`
  
  * Go to http://localhost:8080/javaee7-angular/ (http://localhost:8080/javaee7-angular/)

### Deploy in Glassfish 4.1 ###

  * Open Admin Console (http://localhost:8484/)
  
  * Go to menu "Application" 
  
  * In the button "Deploy..." select the file javaee7-angular.war
   
  * Go to http://localhost:8080/javaee7-angular/ (http://localhost:8080/javaee7-angular/)
  
### Deploy in Embedded-Glassfish 4.1 ###

  * Just run `mvn embedded-glassfish:run`
  
  * Go to http://localhost:8080/javaee7-angular/ (http://localhost:8080/javaee7-angular/)
  
### Run with TomEE ###

  * Just run `mvn tomee:run`
  
  * Go to http://localhost:8080/javaee7-angular/ (http://localhost:8080/javaee7-angular/)
  
## Javascript Package Management (optional) ##

The required JS libraries are included in the project, but it also possible to manage them following the next steps:

* You need NPM. Please go to http://nodejs.org/download/ to get a copy.

* Once NPM is installed run the command `npm install`.

* Install Grunt `npm install -g grunt-cli`  for more information please go to http://gruntjs.com/getting-started.

* Run the command 'grunt' to download all the web dependencies and build an optimized version of the project.
