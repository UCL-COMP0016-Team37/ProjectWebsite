---
layout: page
title: Research
permalink: /research/
---
### Related projects:

We looked at projects that provide a similar solution.

![]({{site.baseurl}}/images/ngo-aid-map.png)

NGO Aid Map [https://ngoaidmap.org/](https://ngoaidmap.org/) is a website that provides tools to find and filter NGO projects. They currently have 988 projects with 66 organizations. Their website allows users to navigate using a map clicking on countries to view the projects there. It also has a search which can filter by sector, location and reporting organization.

![]({{site.baseurl}}/images/ngo-aid-map-search.png)

### Data Sets:

Our client pointed us towards different data sets because their own data was not ready yet. The IATI (International Aid Transparency Initiative) [https://iatistandard.org](https://iatistandard.org) is a global initiative that provides a large amount of data on humanitarian activities. Currently they have over a million published activities to their standard. Their data sets can be downloaded from [https://data.humdata.org/organization/iati?q=&ext_page_size=100](https://data.humdata.org/organization/iati?q=&ext_page_size=100). This data needs to be downloaded for each country so it would be a good idea to automate this.

### Technologies

We knew that we needed the application to be easily accessible by users and so we decided to create a web application. The majority of users would use the application on a laptop or desktop computer although we would like to support mobile too.

We understood we needed to create a frontend for users to interact with and a backend to provide an API for the frontend to manage how users access data.

For the frontend we considered lots of different frameworks including Angular, React and Vue. Ultimately we decided to use React because some of use had some experience with it before and it simplifies creating the website. To create the maps we considered different APIs: OpenLayers, Bing Maps, WebGL, Google Maps. For our prototype we used Bing Maps because it was easy to add points to the map in a JSON format. To help the with designing the frontend we used bootstrap because it gives components that can be used very quickly to improve how a user can use the application.

For the backend we considered many languages and frameworks. Python, JavaScript, Java, PHP and C# were all languages that we considered but we decided that since we all knew Java it would be the best choice. Java Spring Boot was chosen as the framework because it makes it simple to create endpoints for our backend api.