---
layout: page
title: Appendices
permalink: /appendices/
---

### Quick Start Guide for users

#### MAIN / MAP PAGE
Main page shows the number of ngo project around the world which is grouped in a pin. On initial zoom, some countries are grouped together. If the map is zoomed further, the pins will spread to each country in which the user can click to go and view location of each project. If it is then clicked again, user will go to search results page which shows all project in the country.
![]({{site.baseurl}}/images/pin-hover.png)

#### PROJECT PAGE
Project page shows all the details of one particular project. Among the data shown includes, location, reporting organisations, budget, overview and transactions.
![]({{site.baseurl}}/images/project-page.png)

#### TOP 100
Top 100 page shows the list Top 100 donors/reportiong organisations including their number of projects reported.
![]({{site.baseurl}}/images/top-100.png)

#### SEARCH
In search, user can choose to search either by keyword, sectors or country or any combination of all of them. User will then be redirected to the search results page to view the project list.
![]({{site.baseurl}}/images/search.png)
![]({{site.baseurl}}/images/search-result.png)

#### ANALYSIS
Analysis helps aggregate all the data of the search category and graph it so that user would be able to get the general overview of projects in a country or projects in a sector or a combination of both.
![]({{site.baseurl}}/images/analysis.png)
![]({{site.baseurl}}/images/analysis-page.png)

### Deployment manual

#### Frontend
Frontend is deployed based on Node.js server structure and developed using React.js, hence, we use `npm` to deploy and install dependencies.

For running it on the local machines, we needs to do following:
* To install dependencies by running `npm install`
* To deploy to `build` folder by running `npm run build`
* To run locally by running `npm start`

The frontend is available [here](http://mappingtoolfrontend.azurewebsites.net/).


#### Backend
Backend is deployed on **Azure Web** server which and will be automatically deploy for any trigers push on *prod* branch through the DevOp setting on *Azure Pipeline*. 
For local deployments, since *prod* branch is connected to the pipeline, a *master* branch is design for **localhost** running. 

In order to do so, we needs to do following:
* Checkout to a *HEAD* version on *master* branch.
* Have `mvn` installed
* Run `mvn clean package` to download all the dependencies
* Run `mvn spring-boot:run` to start the backend server.

Also, for testing and developing purposes, we design an interactive API Document which is avaliable [here](https://mapping-tool-api.azurewebsites.net/swagger-ui.html#/). 


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

##### Project Website
* Chosen template using Jekyll
* Uploaded Jekyll template to web server

##### Plan
* Create backend API to access data
* Integrate backend API with frontend
* Add search functionality
* Add search filters
* Start creating project website with progress so far
* Add more modes to the map

### 7th February 2020
#### Progress
We made progress in displaying different maps such as a heat map and funding flow map. We also added the ability for the frontend to open and view project pages. Another fix was made to fix eslint on the frontend which was reporting too many errors and being ignored. By making eslint more lenient we improved the quality of the code.
 
#### Frontend
* Added pin map clustering
* Added heatmap
* Added funding flow map
* Added map control panel
* Switched funding flow to be more realistic sample data.
* Added support for viewing IATI project pages
* Changed navbar style
* Improved search results by adding a spinner to indicate they are loading
* Changed search results to use bootstrap cards

#### Backend
* Added unit tests for IATI APIs
* Added publisher API endpoint
* Refactored utility code to improve readability
* Added entities to model the data from the IATI (location, contact info, activity dates, reporting organisation, narratives)

#### Plan
* Add individual project viewer
* Fix advanced filter

### 28th February 2020

#### Progress
We had a meeting with the master’s team working with the ANCSSC to discuss what data we are using and how we are using it with the purpose of integrating. We had a large meeting with the representatives of the ANCSSC and the other 2 groups they are working with. They explained how they expected our projects to integrate. We had not been planning this so far and so we proposed to use the IATI data standard as we already are using it and we revised our MoSCoW list with our new expectations and what is obtainable. We had to decide to not include the funding flow map as most of the IATI data did not have a location for the funder and the recipient and so plotting this wouldn’t appear very informative or useful.
 
#### Frontend
* Designed project page
* Added sections to project page overview, locations, budgets and transactions.
* Redesigned the search bar to have a pop up and more advanced filter options.
* Changed heatmap to be by country region
* Changed maps to use real IATI data from the backend
* Changed how the pin map shows data points and zoom gives more detail
 
#### Backend
* Added map API to get data by country
* Added paging for search

#### Plan
* Add funding flow map

### 13th March 2020

#### Progress
We have been discussing with the ANCSSC about how to integrate our project with the other 2 teams. It is difficult for us because we have been using the IATI standard for our project so far and the ANCSSC data does not exist yet so we can’t test with it. We are communicating with the other teams to design a database to use for the data.

#### Frontend
* Fixed missing location in project page (when projects did not specify location this would crash the page)
* Added mapstyle dropdown on main page to change the design of the map (dark, light, road, satellite)
* Changed mapstyle to dark on the project page
* Redesigned project page to be easier to use and understand
* Added advanced search filters by country and sector
* Fixed project page not displaying narrative if the narrative is not in english instead use the available language
* Fixed bug with forward button on paginated search results allowing the user to click forward on the last page of results

#### Backend
* Added the ability to filter search results and added this to the API doc
* Added the endpoint to view transactions

#### Plan
* Fix bugs
* Improve user interface

### 27th March 2020

#### Progress
The final two weeks have been focussed on fixing as many bugs as possible and improving the usability of the application. We have reimplemented a lot of features that we previously removed such as the funding flow map and the heatmap because we found we could use them effectively on the analysis page. We have created all the surrounding documents as well, including feature video, demonstration video, poster, demonstration slides, project website.

#### Frontend
* Removed funding flow map from home page
* Cleaned up console.logs
* Changed pin colour for different map styles
* Added help page with screenshots and guide on how to use the tool
* Added related activities to project page
* Fit map on homepage to fill window
* Added transactions to project page
* Added top 100 paginated organisations graph
* Fixed npm audit problems
* Redesigned homepage and navbar
* Changed and redesigned search results analysis page
* Readded funding flow inside of analysis
* Added heatmap to analysis
* Fixed edge cases of project page not rendering certain projects
* Redesigned help page
* Fixed deployment

#### Backend
* Added analysis test
* Added recipient graph
* Added sector api and graph analysis
* Added country api and graph analysis
* Added top organisations api
* Added funding flow api
* Added funding flow unit tests
* Refactored
