# Spring Boot and Angular 10 CRUD Tutorial 

 ## Overview 
> In this tutorial, a CRUD (Create, Read, Update, and Delete) application using Spring Boot, Angular, and MySQL is created for an Employee Management system. 
> This system tracks Employee Name and Phone Number, but can easily be modified for further components. 
> 
> The full tutorial can be found [here](./AngularSpringBootTraining.pdf)

## Features 
> * Create an Employee 
> * Update an Employee 
> * List Employees 
> * Delete an Employee 
> * View an Employee

##Client and Server 
> The [springboot2-jpa-crud](./springboot2-jpa-crud) directory develops the CRUD RESTful APIs for the Employee Management System using Spring Boot 2, JPA, and MySQL. 
> The [angular10-client](./angular10-springboot-client) directory develops the single page application, using Angular 10 for front end development in this example. This application consumes the CRUD RESTful APIs developed and exposed by the springboot2-jpa-crud project. 


## Tools and Technologies 
> * Spring Boot 
> * JDK 
> * Spring Framework 
> * Hibernate
> * Spring Data JPA

> ### Database 
> MySQL Database 

> ### Front End Technologies 
> * Angular 10
> * Bootstrap 
> * NPM 
> * jQuery 
> * NodeJS

### Tools
> * Maven 
> * IDE - IntelliJ (Spring Boot API)
> * Visual Studio (Angular Application)
> * Angular CLI 10 


## File Directory 
> ### Spring Boot Server
> #### Controller Layer 
>>[controller](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/controller)
>> * [EmployeeController.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/controller/EmployeeController.java)
>
> #### Exception Handling 
>>[exception](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/exception)
>> * [ErrorDetails.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/exception/ErrorDetails.java)
>> * [GlobalExceptionHandler.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/exception/GlobalExceptionHandler.java)
>> * [ResourceNotFoundException.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/exception/ResourceNotFoundException.java) 
>
> #### Model Layer
>>[model](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/model)
>> * [Employee.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/model/employee.java)
>
> #### Repository Layer 
>>[respository](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/repository)
>> * [EmployeeRepository.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/repository/EmployeeRepository.java)
>
> #### Application Properties 
>> * [application.properties](../angularspringbootcrud/springboot2-jpa-crud/src/resources/application.properties)
> 
> #### Spring Boot Application 
>> * [Springboot2JpaCrudApplication.java](../angularspringbootcrud/springboot2-jpa-crud/src/main/java/net/guides/springboot2/springboot2jpacrud/Springboot2JpacrudApplication.java)

> ### Angular 10 Client 
> #### Application Files 
>> * [angular.json](../angularspringbootcrud/angular10-springboot-client/angular10-client/angular.json)
>> * [index.html](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/index.html)
>> * [main.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/main.ts)
>> * [polyfills.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/polyfills.ts)
>> * [package.json](../angularspringbootcrud/angular10-springboot-client/angular10-client/package.json)

> #### Employee Object
>> * [Employee Object](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee.ts)

> #### Employee Service 
>> * [Employee Service](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee.service.ts)

> #### Create Employee
>> [Create Employee Component](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/create-employee)
>> * [create-employee.component.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/create-employee/create-employee.component.ts)
>> * [create-employee.component.html](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/create-employee/create-employee.component.html)

> #### Employee Details 
>> [Employee-Details Component](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee-details)
>> * [employee-details.component.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee-details/employee-details.component.ts)
>> * [employee-details.component.html](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee-details/employee-details.component.html)

> #### Employee List 
>> [Employee-List Component](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee-list)
>> * [employee-list.component.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee-list/employee-list.component.ts)
>> * [employee-list.component.html](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/employee-list/employee-list.component.html)

> #### Update Employee 
>> [Update Employee Component](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/update-employee)
>> * [update-employee.component.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/update-employee/update-employee.component.ts)
>> * [update-employee.component.html](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/update-employee/update-employee.component.html)

> #### Application Routing 
>> * [app-routing.module.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/app-routing.module.ts)

> #### Application Root Component
>> * [app.component.ts](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/app.component.ts)
>> * [app.component.html](../angularspringbootcrud/angular10-springboot-client/angular10-client/src/app/app.component.html)

> ## Employee Management System 
> ### Home Page
> ![Home Page](../crudexample/img/home.png)
> ### Create
> ![Create](../crudexample/img/create.png)
> ### Read
> ![Read](../crudexample/img/read.png)
> ### Update
> ![Update](../crudexample/img/update.png)
> ### Delete
> ![Delete](../crudexample/img/delete.png)