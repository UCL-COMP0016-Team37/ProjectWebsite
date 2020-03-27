---
layout: page
title: Design
permalink: /Design/
---

### Final Prototype
In the frontend we use make use of separation of concerns and encapsulation by separating our code into components. These components pass props between each other in a tightly controlled fashion using prop types. This makes it easy to expand in the future and very scalable.

When a user first opens the site they are presented with an overview of the data, a map showing the number of projects in different regions. When the user zooms into this map the regions decrease in size allowing the user to see how many projects are in each country. In addition, hovering on top of the pins would show the country name associated with the pins. When the user clicks on a country it opens a page that allows the user to search and analyse the projects in that country.

Another overview chart is the top 100 funders. It shows the list of funders with the number of projects they reported. The chart is paginated, as shown, to display the distribution more clearly.

We designed our frontend to be easy to use requiring no instructions on how to use it however we thought it would be best to provide a help page to help those who need it. The help page explains how to use the major features of the tool including step by step pictures.
Searching is very important when dealing with large data sets. Our search tool allows searching by title and description of activities and also filtering by country and sector. After a search query is sent the search results can be viewed and any of the projects can be opened to view a detailed breakdown on their project page. Alternatively for a search result the user can click view analysis which shows graphs and maps based on the search results. The user can switch the graph type and it will update all the graphs.

On the project page a map displays the location of the activity if it has one. Information is also shown about the activity overview, budgets, transactions, related activities and locations.

For the backend, it serves data to the front end. The API can be queried to retrieve from data sources in JSON format. Also, We have this interactive API document served on the azure server. It provides descent description, data examples and use cases which helps developers to build the front end.



![]({{site.baseurl}}/images/architecture.png)
![]({{site.baseurl}}/images/sitemap2.png)

### First Prototype
Our first prototype tests the essential technologies for our application.
It has a frontend and backend that communicate.
This prototype aims to build a resuable and extendable frontend and backend structure rather than build beautiful UIs and different functionalities.
The main achievement is designing the whole structure of commnication from user all the way for accessing the related data in the database.

### System Architecture Diagram
Here is the diagram of our system architecture which display the communication between frontend (client website) and backend (data server and database):
![]({{site.baseurl}}/images/architecture.jpg)

### Backend
The backend has a SpringBoot api to allow the frontend to communicate with it and a database of over a thousand projects.
Backend is deployed on the **Azure** web server, which includes the web server and database. 
![]({{site.baseurl}}/images/back-azure.jpg)

Backend is visualized by using Swagger by this [link](http://mapping-tool-api.azurewebsites.net/swagger-ui.html#/), this can be very slow to 
access since we use a free server at the prototype page. The UI is as following:
![]({{site.baseurl}}/images/back-ui.jpg)

Current API only support project accessing and user manipulating, however, this provide an extendable structure for future possible functionalities.

### Frontend

The frontend is a React application which includes a map (using MapBox), search and chart which demonstrate the behaviour using sample data.
So far, three functionalities are supported: *Mapping*, *Search*, and *Top 100 Donors*.

Mapping achieves that projects are mapped on the world map and display their current number on that region
![]({{site.baseurl}}/images/front-map.jpg)

Search supports searching a keyword and display the result under a table display.
![]({{site.baseurl}}/images/front-search.jpg)

Top 100 Donor provides the feature of showing a bar chart for the top donor as well as their projects number.
![]({{site.baseurl}}/images/front-top.jpg)

Overall, the current site map demostrates the connnection between pages:
![]({{site.baseurl}}/images/sitemap.png)