---
layout: page
title: Architecture
permalink: /architecture/
---
SPARKR is designed and developed by students under the guidance of professionals from among other IBM.

The architecture of SPARKR is inspired by several design principles:
* Client-Backend,
* Object-Oriented (OO),
* Model-View-Controller (MVC),
* Microservices with REST API,
* Test-Driven Development (TDD),
* Agile,
* Growth Hacking.

What follows is a brief explanation and how this impacts the technologies that we prefer to use.  

## MVC
MVC is an acronym for Model-View-Controller. The main idea behind MVC is that you create

## Client-Backend
The highest level design principle of an application is to think of your system as a Client with a User Interface (UI), also called the Front-end, and a Backend with the heavy lifting of applications running specific calculations.

The Backend has most likely a persistence layer to save the state of data, most often that is in the form of a [Database (DB)](https://en.wikipedia.org/wiki/Database) or a Database Management System (DBMS).

There is a continuing debate about how much code you should allow into the Client and how much code should be implemented in the Backend instead. You will hear the terms '[Thin Client](https://en.wikipedia.org/wiki/Thin_client)' and '[Fat Client](https://en.wikipedia.org/wiki/Fat_client)' (also called think, heavy, or rich). There is no hard definition when a client is thin or thick, but the general rule is that the less logic and calculations you add to the client, the thinner the client is, and the more code, other than HTML and CSS, you add to the client the thicker the client. What makes a client too thin or too thick depends a little bit on:
* how does your client effect the [computer performance](https://en.wikipedia.org/wiki/Computer_performance)?
* how much computing power (CPU, RAM) and storage  does the client have?
* how large is the bandwidth of the internet connection?
* How fast is the internet connection?

With the increased popularity of Mobile as a Client device and the exponential growth of Computer performance (see [Moore's Law](https://en.wikipedia.org/wiki/Moore%27s_law)), the definition of thin and thick has shifted. With the increase in different types of clients (desktops, laptops, browsers, apps, mobile devices, smartwatches, TVs, screen sizes) clients must be designed to be responsive and platform independent. This all caused the popularity of rich client libraries like JQuery, Bootstrap, Backbone, Angular, React. As a principle, I favor thin clients with low network traffic, but there is an immediate tension between the two. The introduction of REST and JSON greatly contributed to balance in favor of thin clients, but frameworks like Angular and React added weight back onto the client. The ideal is a golden middle road, using REST and JSON in thin clients with front-end frameworks like Angular or React.

### Client

The client itself can be further broken up in components. Again, the general rule is to design as modular as possible, creating loosely-coupled modules with as little as possible dependencies. 

#### Front-end Components

* Create the View and static front-end in HTML and CSS.
* Create the front-end Controller in Angular2. The alternative for Angular2 could be React.
* Use TypeScript to create custom components.
* Front-end tools: JQuery,

### Backend


## Object-Oriented (OO),


## Model-View-Controller (MVC),


## Microservices with REST API,


## Test-Driven Development (TDD)

* e2e: Protractor
* Test runner: Karma
* Unit Tests: Jasmine
