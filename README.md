Rules Engine POC API
====================

The rules engine is developed using spring boot and the easyrules library. We have created a dummy json file(offers.json) which includes sample offers. Using the json file we will then validate each offer through the easyrules bean xml(rules-engine-bean.xml) with a set of rules defined by us. Based on those rules the output of offers will defer and will be displayed to the user.    


To run the project
------------------
* Clone the project into your local workspace
* Clean and install project using maven command - `mvn clean install`
* Start the server using - `mvn spring-boot:run`
* Run the application in your local browser specifying the user role as a parameter,

* If `Student` - http://localhost:8080/offer?userRole=student
* If `Teacher` - http://localhost:8080/offer?userRole=teacher

	
* Note that offers will be displayed according to the roles and their specific rules mentioned in the bean xml




