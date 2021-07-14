# Ejercicio Práctico de Lean Tech
No requirement demo project



### What is this repository for?

* Quick summary.

Crear un proyecto en SpringBoot con una base de datos h2(en memoria).
El proyecto debe tener las siguientes entidades: Person, Employee, Position

```SQL
Candidate{
id,
name,
lastName,
address,
cellphone,
cityName}

Employee{
id,
person,
position,
salary}

Position{
id,
name}
```
el servicio debe exponer una API Rest que permita hacer las siguientes operaciones:


* Version.

1.0.0

### How do I get set up? ###

* Summary of set up.
As is.

* Development environment.
- DB:				H2
- Java version: 	1.11
- Maven

* Configuration.
- Install H2 DB


* Dependencies.

this library uses 
- lombok
- Google Guava
- Hibernate?
- H2



* Deployment instructions
- use [maven](https://spring.io/guides/gs/maven/) to compile and run the project.
- Execute REST methods with a platform for REST API development like [Postman] (https://www.postman.com/)
  - *POST: localhost:8080/person/post  
    - <Body raw> 
	JSON: 
	{
 "name" : 'MyName',
 'lastName' : 'MyLast',
 "address" : "245 street, city, state, Ctry 20105",
 "cellphone" : "9152240040"
}
    
  - GET (all): localhost:8080/person/
  - GET (single): localhost:8080/person/{id} example:  localhost:8080/person/1   
  - PUT: localhost:8080/person/put/{id} example:  localhost:8080/person/put/1
	- <Body raw> 
	JSON: 
	{
 "name" : "MyOtherName",
 "lastName" : "myOtherLast",
 "address" : "245 street, city, state, MX 25070",
 "cellphone" : "None"
}
  - DELETE: localhost:8080/person/delete/{id} example:  localhost:8080/person/delete/1
  
  

### Contribution guidelines ###

* Writing tests.

Only some basic Unit testing is setup at the moment.

* Code review.

Request if needed.

* Other guidelines.

Please ask for the code standard to use as guideline and reflect it in the project.

### Who do I talk to? ###

* Repo owner or admin.

owner 		- current main developer - obed.vazquez@gmail.com


