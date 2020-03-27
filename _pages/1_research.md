---
layout: page
title: Research
permalink: /research/
---
### Related projects:

We looked at projects that provide a similar solution.

![]({{site.baseurl}}/images/ngo-aid-map.png)
([https://ngoaidmap.org/](https://ngoaidmap.org/), 2020)

NGO Aid Map [1] is a website that provides tools to find and filter NGO projects. They currently have 988 projects with 66 organizations. Their website allows users to navigate using a map clicking on countries to view the projects there. It also has a search which can filter by sector, location and reporting organization. The drawback of using this is does not provide much data or insight.

![]({{site.baseurl}}/images/ngo-aid-map-search.png)
([https://ngoaidmap.org/](https://ngoaidmap.org/), 2020)

![]({{site.baseurl}}/images/dportal.png)
([http://www.d-portal.org](http://www.d-portal.org), 2020)

d-portal [2] is a website that can browse and analyse the IATI data. The tool allows users to perform search and filter. The search results can then be graphed in different aspects and it generates reports based on the aggregates of different axes. It also allows the user to view individual projects in a clean and easy to understand format. The drawbacks of d-portal is it is hard to use and not user friendly.

### Data Sets:

Our client pointed us towards different data sets because their own data was not ready yet. The IATI (International Aid Transparency Initiative) [3] is a global initiative that provides a large amount of data on humanitarian activities. Currently they have over a million published activities to their standard. Their data sets can be downloaded from [https://data.humdata.org/organization/iati?q=&ext_page_size=100](https://data.humdata.org/organization/iati?q=&ext_page_size=100). This data needs to be downloaded for each country so it would be a good idea to automate this.

### Technologies

We knew that we needed the application to be easily accessible by users and so we decided to create a web application. The majority of users would use the application on a laptop or desktop computer although we would like to support mobile too.

We understood we needed to create a frontend for users to interact with and a backend to provide an API for the frontend to manage how users access data.

For the frontend we considered lots of different frameworks including Angular, React and Vue. Ultimately we decided to use React because some of use had some experience with it before and it simplifies creating the website. React promotes encapsulation by separating out code into components which pass data between themselves in a controlled way which we enforced using prop-types. Prop types would check the type of the props we were passing to our components and throw an error if they didn't match. JavaScript doesn't have any type checking before runtime so this was very useful. To create the maps we considered different APIs: OpenLayers, Bing Maps, WebGL, Google Maps. For our prototype we were using Bing Maps but we changed it to MapBox because it BingMaps did not provide the full functionality that we needed. MapBox gave us the control to add advanced maps such as funding flow and heatmap. To help the with designing the frontend we used bootstrap because it gives components that can be used very quickly to improve how a user can use the application. We used bootstrap for all the buttons, dropdowns and layout. By using a library for style it helps our site conform to web design standards making it more familiar to users.

For the backend we considered many languages and frameworks. Python, JavaScript, Java, PHP and C# were all languages that we considered but we decided that since we all knew Java it would be the best choice. Java Spring Boot was chosen as the framework because it makes it simple to create endpoints for our backend api.

### References

* [1] InterAction. "NGO Aidmap" [Online]. Available: [https://ngoaidmap.org/](https://ngoaidmap.org/) [Accessed March 2020].

* [2] d-portal. "d-portal" [Online]. Available: [http://www.d-portal.org](http://www.d-portal.org) [Accessed March 2020].

* [3] IATI. "IATI standard" [Online]. Available: [https://iatistandard.org](https://iatistandard.org) [Accessed March 2020].