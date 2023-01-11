# Individual Project (Hearthstone Deck Maker)
## Introduction
For my Individual Project I am going to make a Hearthstone Deck Maker. On this web application you can get an overview over all the cards available in the game, get an overview of created decks by all users of the application and a page to create a deck yourself. For the card overview I got my inspiration from the [Hearthstone](https://hearthstone.blizzard.com/en-us/cards?set=standard&sort=dateadded%3Adesc%2Cname%3Aasc%2Cclasses%3Aasc) site.
![Hearthstone Card Overview](https://github.com/S3-HSDM/Portfolio/blob/main/images/cardoverview.jpg?raw=true)

For the deck overview I got my inspiration mainly from [HearthPwn](https://www.hearthpwn.com/decks?filter-show-standard=1&filter-show-constructed-only=y&filter-deck-tag=1) site.
![HearthPwn Deck Overview](https://github.com/S3-HSDM/Portfolio/blob/main/images/deckoverview.jpg?raw=true)

## Learning Outcomes (LO)
For this semester we have to match some learning outcomes. These learning outcomes are displayed [here](https://github.com/S3-HSDM/Portfolio/blob/main/Learning%20Outcomes.md).

## Project choices (LO-6)
For this project I work according to the Agile ideology. I do this by working with Kanban method. Therefor I created a Kanban board on [Github](https://github.com/orgs/S3-HSDM/projects/1). The reason to choose for Kanban come from research I have done towards [Agile (LO-3)](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Agile.md) working. Doing this research and using the Kanban method for my IP helps me demonstrate being proficient for Learning Outcome 3.

The languages and frameworks I use for my Individual Project are Java Spring Boot for the Backend of the project and Javascript Angular for the Frontend. The database will be a MySQL database. The reasoning for choosing these languages/frameworks are further explained in my research files. [Backend](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Java%20Backend%20Research.md), [Frontend](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Javascript%20Frontend%20Research.md) & [Database](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20&%20Documentation/Databases.md).

## Software design (LO-6 & Lo-1)
Before I could start coding for my web application I made Requirements, functional and non-functional. With those requirements I created user stories for my project. After the user stories I created a C4-model for my project. Those user stories and diagrams can be found in my documentation files. Creating the analysis document and researching my project choices help me demonstrate being proficient for Learning Outcome 6.

[Analysis Document](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Documentation.md)

For my UI design I followed the UX Method Competitive Analysis. To achieve this method I took inspiration from the Hearthstone and Hearthpwn web pages shown in the Introduction. For the Card overview page I used the Hearthstone page to find a way to show all the available ways to filter the cards, without creating a chaos of buttons or dropdowns where users could get lost. Also I took inspiration from both sites and want to combine them. On the Hearthstone page is a real good and clear card overview, you can also create decks, but you can't share the deck with others. On the Hearthpwn website is a deck overview page, where you can share your created decks, but you can also get inspiration from others or search for well performing decks. Yet the Card overview page is not clear, the filters are hard to find and you can't pick up all cards at once.

## CI/CD (LO-4 & LO-2)
### CI
To ensure that my project on the main branch is a working version I added CI via Github Actions. Every time something is pushed to the main branch, via a pull request from the development branch, the Github action runs all the tests and Sonarcloud. For my Backend and Frontend it runs a series of Unit tests and Regression test.

![Backend Github Actions](https://github.com/S3-HSDM/Portfolio/blob/main/images/BackendActions.png?raw=true)

The tests running in the backend can be seen [here](https://github.com/S3-HSDM/HSDM-BackEnd/tree/main/hsdm/src/test/java/nl/fhict/s3/hsdm). This folder contains the Unit tests.

![Frontend Github Actions](https://github.com/S3-HSDM/Portfolio/blob/main/images/FrontendActions.png?raw=true)

Regression tests make sure existing features still work when new code is added to the project. These Regression tests are very useful, because you don't have to manually check if the whole project still works when you add a new feature. These Regression tests consist of the Unit tests, which run automatically if new code is push to the main branch, because of the CI pipeline. Creating this CI pipeline helps me demonstrate being proficient for Learning Outcome 4.

For my Non-functional requirements I used Lighthouse. This tool helps improving the performance, quality, and correctness web apps. When the tool audits a page it runs a serie of tests on the page and gives a report on how the page performed. The tool also gives tips to help improve the performance of the page. The first score below is from running lighthouse on the Cards page, with the report and tips on how to improve the page. The other score is from the Home Page.

![Performance Lighthouse Card Page](https://github.com/S3-HSDM/Portfolio/blob/main/images/PerformanceLighthouse.png?raw=true)
![Performance Lighthouse Card Page Improvements](https://github.com/S3-HSDM/Portfolio/blob/main/images/LighthouseImprovements.png?raw=true)
![Performance Lighthouse Home Page](https://github.com/S3-HSDM/Portfolio/blob/main/images/LighthouseHome.png?raw=true)

From the scores I can conclude the performance is massively reduced by unused Javascript and uncompressed text, so fixing those issues would be the next step in improving the performance of my web application to match my requirements.

After researching I found a way to reduce the size of the Javascript by editing configurations in the angular.json and package.json, which changes the way the application gets build, which massively increased the performance for my application.
![Performance Lighthouse Card Page Improvemed](https://github.com/S3-HSDM/Portfolio/blob/main/images/LighthouseImprovemed.png?raw=true)

Running these performance tests and improving my code/performance with this test helps me demonstrate my proficiency at Learning Outcome 2.

### CD
For CD I setted up Docker for my project. Via a Docker-compose file 4 containers are created, one for my Frontend, one for my Backend and two to set up the Database. With those containers running my project runs on localhost. With the Docker images of my project, anyone can run my project on any device. Deploying my project on Docker helps me demonstrate being proficient at Learning Outcome 4.

![Docker Containers](https://github.com/S3-HSDM/Portfolio/blob/main/images/Docker.png?raw=true)

## Software Quality (LO-2)
The tests that I have written for my CI are also a way to ensure the Software Quality of my project. These are automated tests which will run every time new code is pushed to the main branch, ensuring the Software Quality of the main branch. In my CI pipeline I've also integrated a workflow for Sonarcloud. Sonarcloud is a tool that checks my project for clean code, it looks for bugs, vulnerabilities, security hotspots, code smells and duplicated code. Every time new code is pushed to the main branch it checks for these 5 points and returns a report for code to improve, enhancing the Software Quality of my project. The first time I ran Sonarcloud on my project it came up with multiple issues.
![Sonarcloud Before](https://github.com/S3-HSDM/Portfolio/blob/main/images/SonarCloudBefore.png?raw=true)
After checking the report returned by Sonarcloud I improved the quality of the code in my project, resolving the issues found by Sonarcloud.
![Sonarcloud After](https://github.com/S3-HSDM/Portfolio/blob/main/images/SonarCloudAfter.png?raw=true)

Clean code is important for Software Quality as are the automated tests. Another good way to improve the Software Quality are Integration test from Postman. These Integration tests send HTTP requests to the endpoints of my Backend and check if the Backend returns correctly. The tests check if the request returns the correct status code and if necessary if the request returns a body.
![Postman Tests](https://github.com/S3-HSDM/Portfolio/blob/main/images/PostmanTests.png?raw=true)
![Postman Test Results](https://github.com/S3-HSDM/Portfolio/blob/main/images/PostmanRunTests.png?raw=true)

During the last Demo some small issues acted up. The CRUD functions didn't fully react or the backend/database connection wasn't fully working. Now I couldn't identify the root of the problems, which can be annoying to me, but also to other developers who want to work with the code. A good step to improve this and thus improving the software quality would be adding status codes and messages to the API responses. With status codes it gets easier to identify the root of the problems.

Improving Software Quality also includes security testing. Therefor I've tried Cross-site scripting (XSS) on my application. XSS enables attackers to inject malicious code into web pages. Such code can then, for example, steal user and login data, or perform actions that impersonate the user. This is one of the most common attacks on the web. To block XSS attacks, you must prevent malicious code from entering the Document Object Model (DOM). For example, if attackers can trick you into inserting a <script> tag in the DOM, they can run arbitrary code on your website. The attack isn't limited to <script> tags —many elements and properties in the DOM allow code execution, for example, <img alt="" onerror="..."> and <a href="javascript:...">. If attacker-controlled data enters the DOM, expect security vulnerabilities.

![AddCard Function Script XSS](https://github.com/S3-HSDM/Portfolio/blob/main/images/AddCardXSS.png?raw=true)
![AddCard Function Script XSS result](https://github.com/S3-HSDM/Portfolio/blob/main/images/AddCardXSSResult.png?raw=true)
![AddCard Function DropTable XSS](https://github.com/S3-HSDM/Portfolio/blob/main/images/AddCardXSSDropTable.png?raw=true)
![AddCard Function DropTable XSS result](https://github.com/S3-HSDM/Portfolio/blob/main/images/AddCardXSSDropTableResult.png?raw=true)

The Cross-site Scripting tests show that the Injected code doesn't reach the DOM. The injected code doesn't run in the DOM, but is stored as a string in the database. Sonarcloud also scans the code of my application for security vulnerabilities. From Sonarcloud no security vulnerabilities were found in the main branch of the  Frontend and Backend.
  
To take away the security risks for authentication I've made use of a Authenticator. The Authenticator I choose for my project is Auth0. After researching the security risks for implementing authentication myself I made the choice to use an authenticator, after which I researched 5 well known authenticators, resulting in my choice to use Auth0. ![Research report Authentication](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Authentication.md)

Running Sonarcloud every time code is added to the main branch and resolving code smells, bugs and vulnerabilities helps me demonstrate my proficiency at Learning Outcome 2.

## Web application (LO-1)
For my IP I have created a full-stack web application, Hearthstone Deck Maker (HSDM). Sadly I haven't been able to implement all the user stories I came up with, but the application contains fully functional CRUD operations for the Card entity. All users are able to see all the cards (Read), but when a user is logged in as an admin he is also able to Create Cards, Update Cards and Delete Cards. To be able to distinguish the normal users from the admins I've implemented an external Authenticator named Auth0. Creating this full-stack web application helps me demonstrate my proficiency at Learning Outcome 1. The code for my application are available here. [Backend](https://github.com/S3-HSDM/HSDM-BackEnd) & [Frontend](https://github.com/S3-HSDM/HSDM-FrontEnd)

## Professional (LO-8)
To optimize my IP I have done research into new technologies, research to decide the right languages and frameworks and research to implement secure authentication for my application. Those research reports are available [here](https://github.com/S3-HSDM/Portfolio/tree/main/Research%20%26%20Documentation). Further I have had weekly meetings with the stakeholder and discussed the progress and which steps to take next. The Feedback of those meeting can be found [here](https://github.com/S3-HSDM/Portfolio/blob/main/images/FeedPulse.pdf). Doing these researches and having weekly meetings with the stakeholder help me demonstrate being proficient at Learning Outcome 8.
