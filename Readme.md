#ENSAI JaxRS Lab


The goal of this lab is to add support of restful webservices for an application. 

In order to initialize your project, we provide a tiny sample project to show how to run an JAX-RS application, embedded in Undertow app server, fired up in a `main()` method. 

Undertow is a flexible performant web server written in java, providing both blocking and non-blocking API’s based on NIO.

Undertow has a composition based architecture that allows you to build a web server by combining small single purpose handlers. The gives you the flexibility to choose between a full Java EE servlet 3.1 container, or a low level non-blocking handler, to anything in between.

Undertow is designed to be fully embeddable, with easy to use fluent builder APIs. Undertow’s lifecycle is completely controlled by the embedding application.


### Getting started. 

Fork this project. 

Just build the project:

    mvn clean install
    
and launch the server:

	using the main app
   
You can test the service using 
to get a person
> curl -H "Content-Type: application/json" -X GET http://localhost:8080/status/person

to insert a Person
> curl -H "Content-Type: application/json" -X POST -d '{"name":"test","firstName":"t"}' http://localhost:8080/status/person

You can import this maven project in your favorite IDE. 