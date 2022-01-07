# Spring Boot Notes

The Spring Framework is an application framework that lets you write enterprise-scale Java applications.

Spring Boot is a set of tools to quickly bootstrap a Spring application.

## Spring

Spring has its origins in the concept of dependency injection but it also does much more. Spring helps solve common problems.

Spring has a programming and configuation model, letting you focus on business-specific concerns.

Spring lets you build classes with annotations which denote what they are. For example, you write a business service with the logic specific to your business application, annotate it with `@Service`, and Spring knows to manage this class as a service.

Spring also provides infrastructure support, such as connecting to a database.

Over time Spring has grown into an ecosystem of projects, from Spring Security to Spring Cloud.

### Benefits of Spring

- Application context and dependency injection
- Data access APIs
- Spring MVC

Spring helps with handling interrelated dependecies among objects. It wraps your application in a wrapper, the Spring Application Context, and manages object instances. Every class declares the dependencies it needs and Spring injects those dependencies to make sure that every object has references to all the other instances they require.

The vast majority of applications need to connect to a database. The traditional way to connect to a database in Java was to use JDBC (it's not very pleasant). Spring provides data access APIs for connectivity, querying, and transaction management.

Many enterprise applications are web applications and need to either serve dynamic web pages or expose REST APIs. Spring provides a web framework, Spring MVC, to let you more easily do this.

### Problems with Spring

- Since Spring tries to address many common concerns, it has become a huge framework.

- There a multiple setup steps and a lot of configuration.

- There are also multiple build and deploy steps.

The capability and flexibility of Spring comes at a cost; you need to do quite a bit of work to get it to precisely meet your needs.

It can be difficult to descide on best pathways and practices.

Spring Boot attempts to abstract away these setup and configuration concerns.

## Spring Boot

Spring Boot makes it easy to create standalone, production-grade Spring-based applications that you can "just run".

Spring Boot is opinionated and favours convention over configuration.

Spring Boot generates a standalone application that you can just run (you don't need to configure and deploy a container).

Spring Boot is production ready.

## Java Dependencies

Maven is a build automation tool that lets you declare in a single file, pom.xml, all the dependencies you need. Maven will download the dependencies and add these jars to the class path.
