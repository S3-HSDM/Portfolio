# Group Project for World of Content; The Webshop Scraper Is-It-Live

## Cultural differences and ethics (LO-5)
For cultural differences and ethics to some ethical questions in the world of software development and questioned myself where I draw the line for developing software like facial recognition and ownership of personal data and the protection of this data, but also the design of webpages, which can be misleading or addictive. After that I evaluated my own project for ethical questions.

[Cultural differences & Ethics](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Cultural%20differences%20and%20ethics.md)

## Business processes (LO-7)
For business process I did research towards what a business process is. After the research I created a business process for a customer buying a product in a webshop, but since this process only describes 1 person who is also not part of the business, it didn't really describe a business process. That's why I visualized another business process of our group project. 

[Business Processes](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Business%20processes.md)

## Agile method (LO-3)
To work Agile I have done research towards the principles of working Agile and the different ways to execute this.

[Agile](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Agile.md)

# Group project for World of Content (WoC)
## Agile (LO-3)
As a team we chose to work the SCRUM agile method. So on a daily basis we had several meetings and created an environment where we summed up all of the issues withing the project. Every meeting we took the time to look at the issues and speak up your mind about problems that we were having. That meant that we could all help eachother out and work out the issues one by one.

## Issues
We created issues to keep track of all the things that we need to do as a team, to finish the project. Everyone can create issues, not everyone can assign them to one another. Every issue comes with it's own description and checklist of things that must be done to finish the issue.
![Issues](https://github.com/S3-HSDM/Portfolio/blob/main/images/Issues.png?raw=true)

## Working as a team  (LO-3 & LO-8)
We managed to make it work as a team by making use of the agile method: SCRUM. Also by communicating to one another and having meetings offline- aswell as online. If anyone of us had a problem that we faced, there was always someone to help out and eliminate the issue. Before we started working on the project, we looked at everyones needs and what they wanted to do within the project. For example, Dirk and i are more interested in the frontend and dus React JS, so we started working on that. While te other team members decided to be more involved in the backend of the project, which worked well. Eventually we mamaged to make great progress every sprint and show WoC that we were able to create a webapp based on their requirements.

### What went right?
To be fair we actually managed to do pretty well as a team and split the issues among us all. The communication was great and everyone was excited to work on the project. Creating the issues and working with GitHub to have insights into eachoter's work was also a good thing. We Helped eachother out where we could and made great progress all along.

### What went wrong?
There were one or two sprint assignments where we had to show what we've been working on, but we did'nt prepare ourselfs well enough. Which lead to all being muted when we sat down and just staring at the one team member that brought the laptop to start talking. So, that was'nt so great. We did manage to create time to prepare ourselfs better for the next assignment.

## Requirements & User stories (LO-6)
After we received the assignment, we discussed with our team what we thought was the right thing we had to build. To achieve this we created requirements, functional and non-functional, and User Stories. After the first sprint we discussed those requirements and user-stories with the stakeholder, which resulted in a degree of importance to implement the user stories and requirements.

### Requirements
#### Functional
- Importing the data (Must have) 
- Read the data (Must have) 
- Synchronise data with the retailers data (Must have) 
- An User has to be able to create an account (Could have) 
- An User has to be able to login (Could have) 
- Switch pages to other languages (Could have)
- Store proucts in the database (Could have) 

#### Non-Functional
- Displaying the synced data in graphs.
- The data synchronisation has to be done within 5 minutes.

### User Stories
- As supplier I want to be able to select a retailer to be able to check an overview of the products (must)
- As an user I want to be able to get the result to know if my products are online with percentage of how many are online (must)
- As an user I want to to have an graph on the overview for a quick check to see how many of my products are online (must)
- As an user I have to be able to login to have access to my credentials (should)
- As an user I want to be able to create an account and get access to the application (should)
- As an user I want to be able to set the application to another language when I'm not capable enough to read/understand English (should)
- As an user I want to be able to compare multiple retailers, so I can see which retailer performs best in getting the products live (could)
- As an user I wnat to be able to import products to synchronise (could)

## Workflow
### How does the system work?
You begin at the home page, where you are pesented a dropdown component where you select a retailer from. In this case, we limited the list of options to two retailers, Albert Heijn and Jumbo.

![Select Retailer](https://github.com/S3-HSDM/Portfolio/blob/main/images/SelectRetailer.png?raw=true)

After selecting one of these options, the page will redirect to the main page loaded in with the corresponding data based on what retailer was chosen. You can see an overal score in the progress bar on the top of the page, which represents the score of all products shown in the table. The table on the page is loaded with all the products that the retailer has in stock, where you are able to see what livescore every product has.

### Widgets
We decided to go with several components on a dashboard- like design, which we call widgets. These widgets each contain something different to show. The page consist out of the following widgets:

### Live & Not Live - Score
This widget contains a progressbar where the overal live and not live score has been stacked into. This widget provides an easy overview to all of the products their average livescores.
![Live or Not Live Widget](https://github.com/S3-HSDM/Portfolio/blob/main/images/LiveNotLive.png?raw=true)

### Total amount of products
This widget contains the exact amount of products that the chosen retailer has in stock.
![Total Amount of products Widget](https://github.com/S3-HSDM/Portfolio/blob/main/images/TotalAmount.png?raw=true)

### Products list
This widget contains a table which is filled with products that the retailer has in stock. The table consist out of the following columns: EAN-number, Product description, Status (Live or not live) and the similarity score (How much is the product alike with the provided example).
![Products Table](https://github.com/S3-HSDM/Portfolio/blob/main/images/ProductsTable.png?raw=true)

## Backend
For the logic for this project we created a RestAPI and two scrapers. We also worked with MongoDB to create schemes and save necessary data into the database. For the database we created an ERD diagram, so the one creating the Backend knows which entities to expect and to store from/to the database.

![ERD diagram](https://github.com/S3-HSDM/Portfolio/blob/main/images/DatabaseERD.png?raw=true)

### Scrapers
Two of our team members were frocussed on building scrapers so we could get the necessary data from the retailer's websites. The scrappers simply look over to one of the retailer's page and checks what is on it. It then scrapes the data and puts it into a file. That data we can compare with the list of products data we got from WoC.

### RestAPI
The restapi is a backend tool where we can fetch data to be shown on the frontend of the project. The special thing within this RestAPI is that we managed to create a wrapper to fetch data more easily, instead of working with axios posts and gets.

## Frontend
### Design
To make sure we would build the right thing, we first created wireframes for the pages we thought would be necessary. After discussing those wireframes with the stakeholder we've used their feedback, which resulted in the design we've come up.
![Homepage WoC](https://github.com/S3-HSDM/Portfolio/blob/main/images/HomePageWoC.png?raw=true)
![Resultpage WoC](https://github.com/S3-HSDM/Portfolio/blob/main/images/ResultPageWoC.png?raw=true)

We decided, after discussing design with the stakeholder, to go for a dashboard like style. This because we then could add several widgets, which seem to work quit well with this project. At first we started of with a neutral page, which showed several components. After getting some useful feedback from WoC, we decided to go for the dashboard style. The colors used on the page and in the components work wel with eachother, you can see what is non-functional and what is functional on the webpage. There was a little bit of research needed to see what kind of styling would be best for this project. This depended on what kind of data we where going to show and what kind of components the data was loaded in. We also decided to make use of Bootstrap and build the page using React JS.

### Bootstrap
Bootstrap has a very easy to use and user friendly system, called the Grid system. This system was very useful to us because we wanted the dashboard type of layout, and this was very easy to implement. You could add Containers, Rows and Columns to create a nice layout which was also responsive.

## Livescore
The livescore is momenteraly calculated by comparing one snapshot to the existing list of products. It checks for three different things: EAN-number, Title & Description (bullet points) If any of these don't compare to the ones in the products list, we re-calulate the score and show it on the front of the page.
![Similarity Score](https://github.com/S3-HSDM/Portfolio/blob/main/images/SimilarityScore.png?raw=true)

The livescore is calculated in the frontend of the project, since it doesn't need to be saved in the backend database.

### Software Quality (LO-2)
For the quality of the RestAPI we have created Postman tests to ensure the endpoints are working. We also have deployed the project on Docker in 4 containers: Frontend, Backend, Database and one for the Scrapers. Furthermore we have created for both Scrapers a statistics page, which quickly shows the performance of the Scrapers and if the Scrapers are still working correctly.

### Docker (LO-4)
We have also deployed our Is-It-Live project with Docker. We have created a Docker-compose file which creates 4 containers, 1 for the Frontend, 2 for the Backend (1 for the logic and 1 for the Scrapers) and 1 for the Mongo Database.
![Docker Containers](https://github.com/S3-HSDM/Portfolio/blob/main/images/DockerWoC.png?raw=true)

### My contributions to the group project (LO-1)
I've mostly worked on the Jumbo webscraper for our Is-It-Live application. We as a group have chosen to create the Backend including the webscrapers in NodeJS. The scraper first gets the EAN-number of a product from the database. With this EAN-number it searches the Jumbo productID via an API. With this productID the scraper can find the correct webpage of the product and scrape the productinformation from the page. With this information a product snapshot is created, which is stored in the database.

To check if the scraper is still working correctly and to check the statistics of the process I've also created a statistics page for the Jumbo scraper. This page checks if the Jumbo scraper scrapes the correct page by checking the given EAN-number and the found EAN-number on the page and it keeps track of the time the scraper takes to scrape the products.
![Jumbo Statistics Page](https://github.com/S3-HSDM/Portfolio/blob/main/images/JumboStatistics.png)

Although it gives you all the information it needs, the page could be more user friendly. Improvements for this statistics page could be the use of colors, if an EAN-number doesn't match, make the table cell red and if they do match, make it green. Also the application doesn't really give you the total time of the process, but only a starting time and the time of the product it found last. This could also be displayed as a process time.

In the table overview it is shown the scraper does it's job well. The product it can find have matching EAN-numbers and the product which it says isn't online is also not possible to find in the Jumbo webshop.

Furthermore I have worked on the Backend, creating a functional endpoint to add the products to the database and I've created an seeder thats adds the Jumbo products to the database. I've also worked on the Frontend, creating the PageNotFound page and the RetailerNotFound page and setting up the routing for these pages.
