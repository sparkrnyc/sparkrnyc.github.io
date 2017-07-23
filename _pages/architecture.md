---
layout: page
title: Architecture
permalink: /architecture/
---
SPARKR is designed and developed by students under the guidance of professionals from among other IBM.

The architecture of SPARKR is inspired by several design principles:
* Client-Backend,
* Object-Oriented Programming (OOP),
* Model-View-Controller (MVC),
* Microservices,
* Test-Driven Development (TDD),
* Agile,
* Growth Hacking,
* Offline First,
* Open Source Software (OSS).

What follows is a brief explanation and how this impacts the technologies that we prefer to use.  

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

The client itself can be broken up in components. The general guideline is to design a system as modular as possible, with loosely-coupled modules and as little as possible dependencies between the different modules.  

#### Front-end Components

* Create views or web pages as static HTML and CSS.
* Angular is a front-end component that functions as a Controller to include front-end logic related to each page or view in the UI. Angular also adds so-called [data-binding](https://en.wikipedia.org/wiki/Data_binding), so that you don't need to program JavaScript code in the front-end to create HTML tags for each of the data elements in JSON. An alternative for Angular2 is React.
* Use TypeScript to create custom components.
* Front-end tools: JQuery, Bootstrap.

### Backend

The backend or server itself can also be broken up into different types of servers. Separate functionality should be running on its own server. Examples of types of servers are:

* Proxy server,
* Web server,
* Admin server,
* CDN server,
* File server,
* Application server,
* Image server,
* Object Storage server,
* Database server,
* Business Intelligence server,
* Matching server, etc.

## Object-Oriented Programming (OOP),

In [Object-Oriented Programming (OOP)](https://en.wikipedia.org/wiki/Coupling_(computer_programming)) or [Object-Oriented design](https://en.wikipedia.org/wiki/Object-oriented_design) is a software design method where the system is represented by interacting objects. Objects or classes consist of properties or attributes to store state and methods or actions to interact.

## Model-View-Controller (MVC)

MVC is an acronym for Model-View-Controller. The main idea behind MVC is a type of [coupling](https://en.wikipedia.org/wiki/Coupling_(computer_programming)) where you separate the Model, View and Controller in an application. In MVC, Model, View and Controller work loosely coupled and work independently, without relying on each other. The opposite of [loose coupling](https://en.wikipedia.org/wiki/Loose_coupling) is tight coupling, where the different components of a system heavily depend on each other.

* The Model manages the data, logic and rules of the application, and stores the state of the model.
* The View is the representation layer, or the UI or front-end of the application.
* The Controller accepts input and processes output, and converts commands for the Model or View.

## Microservices

TBD

## Test-Driven Development (TDD)

TBD

* e2e: Protractor
* Test runner: Karma
* Unit Tests: Jasmine

## Agile

TBD

## Growth Hacking

TBD

## Offline First

The Offline First approach to application development recognizes that network downtime is a fact of life. When you develop an Offline First application, you write your app as if it has no internet connection. Once your app works offline, add whatever network functionality you need for your app to do more when it’s online.

* Offline First apps enable data to be written locally first, which is faster than writing directly to cloud services. Having data on hand natively means fewer performance disruptions when networks go down.
* Being offline shouldn't be an error condition. Offline First apps allow your users to work offline or with limited connectivity, by retaining core app functionality at all times.
* By reducing the number of requests to the cloud service, Offline First apps help your app to be more efficient with battery resources and bandwidth usage.

## Open Source Software (OSS)

TBD
