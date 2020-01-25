---
layout: page
title: Prototype
permalink: /prototype/
---

Our first prototype tests the essential technologies for our application.
It has a frontend and backend that communicate.

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