---
layout: page
title: Evaluation
permalink: /evaluation/
---

### Achievement Table

<table>
<tr><th>Requirement</th><th>Importance</th><th>Completed</th><th>Contributors</th></tr>
<tr><td>Mapping tool that shows position of projects around the world.</td><td>Must</td><td>Yes</td><td>All</td></tr>
<tr><td>Search and filter projects by criteria.</td><td>Must</td><td>Yes</td><td>All</td></tr>
<tr><td>Filter all maps by thematic area.</td><td>Must</td><td>Yes</td><td>All</td></tr>
<tr><td>Filter all maps by funder.</td><td>Must</td><td>No</td><td>All</td></tr>
<tr><td>Visualize category of funding.</td><td>Must</td><td>Yes</td><td>All</td></tr>
<tr><td>Visualize where and who donations are from.</td><td>Must</td><td>Yes</td><td>All</td></tr>

<tr><td>Use data from IATI.</td><td>Should</td><td>Yes</td><td>Yangtao</td></tr>
<tr><td>Distinguish and track data licensing so may be filtered and disclosed to the user.</td><td>Should</td><td>No</td><td>All</td></tr>
<tr><td>Point map of locations for projects being carried out.</td><td>Should</td><td>Yes</td><td>All</td></tr>
<tr><td>Display points grouped by nation and zoom in to see sub-national (like NGO aid map).</td><td>Should</td><td>Yes</td><td>Afiq,Ruairidh</td></tr>
<tr><td>Map distribution of thematic areas.</td><td>Should</td><td>Yes</td><td>All</td></tr>
<tr><td>Map top 100 donors / donor countries.</td><td>Should</td><td>Yes</td><td>Afiq,Ruairidh</td></tr>
<tr><td>Generate graphs based on search.</td><td>Should</td><td>Yes</td><td>Afiq,Ruairidh</td></tr>
<tr><td>Generate graphs for individual project.</td><td>Should</td><td>Yes</td><td>Afiq,Ruairidh</td></tr>

<tr><td>Be open public tool rather than a private tool used only by the ANCSSC.</td><td>Could</td><td>Yes</td><td>All</td></tr>
<tr><td>Map funding flow donations.</td><td>Could</td><td>Yes</td><td>All</td></tr>
<tr><td>Login to view different licensed data.</td><td>Could</td><td>No</td><td>All</td></tr>

<tr><td>Map projects of members of ANCSSC.</td><td>Wish</td><td>No</td><td>All</td></tr>
<tr><td>Update custom data</td><td>Wish</td><td>No</td><td>All</td></tr>
<tr><td>Substitute sample data (IATI) with real member data.</td><td>Wish</td><td>No</td><td>All</td></tr>
</table>

<p>
    Note : After researching and discussing with our client, we are no longer required to do the login and license filtering as the functionalities will be handled by the master's team during integration.  Instead, we are required to add ability to show the pin in different kind of map such as satellite map.
    In addition, the filter by funder is not possible due to the limitation of IATI cloud which does not provide the functionalities for us to obtain such kinds of data quickly to serve the frontend.
</p>

### Bug List
<table>
<tr><th>ID</th><th>Description</th><th>Priority</th><th>Resolution</th></tr>
<tr><td>1</td><td>react-bing-map does not support dynamic mapping</td><td>High</td><td>Switched map library to mapbox</td></tr>
<tr><td>2</td><td>IATI activities that contain slashes are not supported</td><td>Medium</td><td>Filtered these activities</td></tr>
</table>

### Contribution Table
<table>
<tr><th>Work packages</th><th>Afiq</th><th>Ruairidh</th><th>Yangtao</th></tr>
<tr><td>Client liaison</td><td>33%</td><td>33%</td><td>33%</td></tr>
<tr><td>Requirement analysis</td><td>33%</td><td>33%</td><td>33%</td></tr>
<tr><td>Research</td><td>60%</td><td>20%</td><td>20%</td></tr>
<tr><td>UI Design</td><td>40%</td><td>60%</td><td>0%</td></tr>
<tr><td>Frontend Programming</td><td>50%</td><td>50%</td><td>0%</td></tr>
<tr><td>Backend Programming</td><td>0%</td><td>0%</td><td>100%</td></tr>
<tr><td>Testing</td><td>25%</td><td>25%</td><td>50%</td></tr>
<tr><td>Bi-weekly Report</td><td>25%</td><td>50%</td><td>25%</td></tr>
<tr><td>Website Editing</td><td>33%</td><td>33%</td><td>33%</td></tr>
<tr><td>Video</td><td>15%</td><td>15%</td><td>70%</td></tr>
<tr><td>overall</td><td>33%</td><td>33%</td><td>33%</td></tr>
<tr><td>Roles</td><td>Frontend and researcher</td><td>Frontend and Website Management</td><td>Backend and video editor</td></tr>
</table>

### Evaluation of project

#### User Interface
The user interface has good parts and parts that can be improved. We wanted to minimise the number of interactions a user had to complete to achieve a certain goal and most of the interface achieves this. From the homepage the user can navigate to all of the most useful features: top 100, search, pin map and help. We also tried to emulate the design of other websites so that users who have experience with other websites will find it familiar and easy to use.

One place the interface could be improved is the search. When a user clicks on the search input field instead of typing in this field a modal appears and they type in this instead. This was added because we wanted to add filters that were easy to use and obvious how. The sacrifice is the misdirection when the user clicks search and they have to shift their gaze from the top right of the screen to the middle. An improvement could be to have the filters appear below the search box when it is clicked and have the search box not move at all.

The top 100 was challenging because we were had to compress a lot of information. By using pages it made the graph more readable and the scale is not blown out by the largest one.

The search results page clearly shows the results and the view analysis button takes the user to the analysis page. It could be more helpful if there is more information for each of the search results rather than just the title.

The analysis page displays a lot of useful information. It could be improved by better showing what the user searched for and allowing more control over what types of graph are displayed and how they are displayed for example what axis they are plotting.

#### Functionality
Our project contains most of the functionality that we intended to implement. There are some parts of the project that we initially thought we could implement but as we ventured through the project it became apparent we could not. One of these is the funding flow map. We wanted to create a map on the front page that had lines from a funder to the organisation they fund. We build this but when we applied the data to it we found the majority of projects and funders did not specify their location. This meant we had an incredibly small sample of the total projects and funders and we felt it wasn't representative of the overall data. We instead re used this component in the analysis page.

#### Stability
Some parts of our project are very stable some are not. One of the less stable parts of the project is the activity page. This page displays a lot of detailed information about any project. The difficulty arises because even though we are using the IATI standard. The standard is very lenient. Projects differ greatly. Our solution was to try and grab certain bits of information and wrap them in try catch blocks so that if they didn't exist we would return an fallback string. This works nicely although there are so many projects with different ways of storing their information it is likely that some are less than optimal. They could have important information missing which is stored in a part of the data structure we are not checking. This can be improved over time by looking at specific examples of projects that do not render well.

#### Compatibility
When we were first asked to build this project for the ANCSSC we were asked to use IATI data and later they might change it to use their own private data but they had not yet collected their data. We later found out that 2 other groups would be extracting this data via forms and pdf extraction to a database and that we were supposed to use their data. We looked into this and had been building our system for data in the IATI standard up to this point. We concluded that our project is compatible with the ANCSSC data because we can use transformers to transform the data into the IATI standard which is a less specific standard than the standard determined by the other groups. We continued to use IATI data because the ANCSSC data was not available and we wanted to be able to test and run our project on data.

#### Maintainability
Throughout our project we have aimed to encapsulate our code so that changes in the future could be made to one system without having to change all the systems. We believe we have achieved this. Our Java Spring Boot backend uses MVC and separates the different endpoints making it simple to add new ones or modify the current ones. The frontend React uses components to separate out the code. Each component had specified prop types making it clear how to pass props between them.

#### Project Management
We have been communicating with and getting feedback from Matt as we progressed through the project. The only improvement to be made here is that we would have liked to know that we were working with 2 other teams at the start.


### Future work
If we had another 6 months we would have liked to implement more maps and visualisations. These would be maps to show different statistics such as budget, transactions, status of the project. Another feature we would like to implement is the usage of the ANCSSC private member data. It has not been collected yet but it would be very useful as the data should be more consistent and higher quality than the IATI data. Overall we have laid a solid foundation and we have designed systems that are expandable and organised for future developers to add to.