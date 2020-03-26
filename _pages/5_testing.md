---
layout: page
title: Testing
permalink: /testing/
---
### Testing Strategies
Our testing strategy is to iterate quickly and seek constant feedback on changes that we make. For example we test as much of the data as possible to find edge cases where we can improve our application. There could be a project that has important information that we would have left out had we not caught it by testing. We write unit tests for the backend and run them before deployment to ensure it has the intended functionality. We also test every feature extensively for how users interact with it and how we can optimise the tool for the user.

#### Unit Test & Integration Test
Unit test is a level of software testing where individual units and components of a software are tested. The purpose is to validate each unit of the software performs as designed. In our case, it is mainly used for the backend API provider. Since Spring boot is used, which is a highly mature and integrated framework, we do not need to focus on the performance of each tiny component but only for the specific procedure (i.e. each API functionalities). 

In practice, we used the ‘Spring Boot Test’ which is embedded into the Spring Boot Framework and ‘JUnit’ for each test case. They test each case of the API performances, specifically, database connections and grab data from IATI Cloud. For database, it mock the repository (terminology for data source in Spring boot) and test the performance of obtaining the data from the database or inserting it without modified the database. The logic of each api functionality is pretested in JUnit before it goes to real service and controller.

Since Spring boot is a mature framework and the integration is defined by annotations (@Service, @Repository and @Controller etc) and it works in ‘Dependency Injection’, there is no need to do integration tests for these components, if proper annotation is used and built.

#### System Test
Our system is separated into two parts, frontend (JavaScript React) and backend (Java Spring boot). The things we need to ensure are the data transmissions. Since it works through HTTP and Json is used for transferring the data, we only need to test if the data sent from the backend can be received properly in the front end.

We used a sample project controller with some fake data as a test for basic functionalities. Using this sample data we can test the frontend accepts this and from this so long as the backend data is in the same structure it will be accepted in the frontend. If the backend data needs to be in a different structure we would need to change the sample data to ensure the frontend accepts it.

#### Performance test
We could test the time for API requesting (Swagger has a response time entity for every API), and every page response time for the frontend. This would help us to identify bottlenecks in our performance and introduce caching strategies for systems that do not change regularly and take a long time to run.

#### User acceptance Test (add more description)
We asked users to use our site by watching and asking them questions we could identify how they used the site versus how they wanted to use the site. We could then take these results and try and remove the difference.
We also got feedback from our project partner and teaching assistants. Our project partner mostly agreed and was satisfied with our design and functionalities. We would also discuss new features and we could hear the feedback about how useful they think they would be.
We got feedback about the how users used the site regularly. With this feedback we made many revisions and redesigns to improve the usability and how intuitive the tool is. 

#### Responsive design testing
We determined early on that our tool would have to work on computer screens. We chose not to build it for mobile because it would be very difficult to display quality, detailed data on a small display and our client did not require it. We designed the website for 
