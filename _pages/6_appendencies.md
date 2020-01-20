---
layout: page
title: Appendices
permalink: /appendices/
---

### Deployment manual

#### Frontend

First run to install dependencies:
#### `npm install`

To deploy to `build` folder:
#### `npm run build`

To run locally:
#### `npm start`


#### Backend

### Bi-weekly reports

#### 21st November 2019
##### Progress

After completing our Prevision coursework we started on the main coursework the mapping project for the ANCSSC.

We have been collating and organising the requirements for the project. We have also been deciding about the technologies we are going to use. We know we need a frontend and backend. The frontend for the user to interact with and the backend to supply data to the frontend. We have decided to use React for the frontend over angular or Vue because some of us are familiar with it already. We also need a map api to display the maps we have chosen to use Bing Maps as their is a React package for it. For the backend we have decided to use Java and SpringBoot because we have all done Java last year on our course. SpringBoot is the most popular Java web framework.

##### Plan
The plan for the next few weeks is to create git projects, the frontend (React) and backend(SpringBoot). We will also configure the devops for the frontend and backend.

#### 5th December 2019

##### Progress
We have started building the initial prototype of the web application and deploying the application on Microsoft Azure. We planned the interaction between the frontend and the backend with a list of API endpoints and what their response will be. Also, we considered the pages the user will interact with and how they should link together.

##### Frontend

* Created react site
* Created repository
* Put react site onto Microsoft Azure
* Basic site routing for different pages
* Created map page
* Created data page
* Created search results page
* Created error page
* Implemented a search bar which takes the user to a page that will have the search results
* Embedded Bing maps widget into the main page of the site
* Added sample markers onto the Bing map of projects around the world

##### Backend
* Created java spring boot web server
* Created repository
* Put web server onto Microsoft Azure
* Dev ops
* Made API docs

###### Project Website
* Chosen template using Jekyll
* Uploaded Jekyll template to web server

###### Plan
* Create backend API to access data
* Integrate backend API with frontend
* Add search functionality
* Add search filters
* Start creating project website with progress so far
* Add more modes to the map 