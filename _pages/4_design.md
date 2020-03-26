---
layout: page
title: Design
permalink: /Design/
---

When a user first opens the site they are presented with an overview of the data, a map showing the number of projects in different regions. When the user zooms into this map the regions decrease in size allowing the user to see how many projects are in each country. In addition, hovering on top of the pins would show the country name associated with the pins. When the user clicks on a country it opens a page that allows the user to search and analyse the projects in that country.

Another overview chart is the top 100 funders. It shows the list of funders with the number of projects they reported. The chart is paginated, as shown, to display the distribution more clearly.

We designed our frontend to be easy to use requiring no instructions on how to use it however we thought it would be best to provide a help page to help those who need it. The help page explains how to use the major features of the tool including step by step pictures.
Searching is very important when dealing with large data sets. Our search tool allows searching by title and description of activities and also filtering by country and sector. After a search query is sent the search results can be viewed and any of the projects can be opened to view a detailed breakdown on their project page. Alternatively for a search result the user can click view analysis which shows graphs and maps based on the search results. The user can switch the graph type and it will update all the graphs.

On the project page a map displays the location of the activity if it has one. Information is also shown about the activity overview, budgets, transactions, related activities and locations.

For the backend, it serves data to the front end. The API can be queried to retrieve from data sources in JSON format. Also, We have this interactive API document served on the azure server. It provides descent description, data examples and use cases which helps developers to build the front end.



![]({{site.baseurl}}/images/architecture.png)
![]({{site.baseurl}}/images/sitemap2.png)