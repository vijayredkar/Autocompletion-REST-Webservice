# Autocompletion-REST-Webservice
REST webservice built with Spring Boot-JPA-BasicAuth to provide data for autocompletion of search text

To launch the service

1- extract the "autocomplete" directory from the zip attached in the email and save it to a local directory

2- in the command prompt navigate inside the "autocomplete" dir.

3- run the command         mvn spring-boot:run

4- once the service is up and running, it can be tested using POSTMAN REST client.

5- Sample test GET URI -     localhost:8080/suggest_cities?start=c&atmost=7

6- this app is secured using BASIC AUTH, hence set the Authorization credentials in POSTMAN to 
   Username = appuser
   Password = password

7- submit the GET URI and verify the results displayed in POSTMAN and the response HttpStatus
   
   sample output 

	Chichdhari Khanapur B.O

	Chintaguda B.O

	Coal Chemical Complex S.O

	Chakepalli B.O

	Chinnoor S.O

	Chintakunta B.O

	Chityal B.O
	
8- this app uses HSQL DB and JPA. Loads cities data at the application start up

9- unit tests are provided for the service and the controller APIs and have good coverage.

10- appropriate exception handling is also provided
