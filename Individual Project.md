# Individual Project (Hearthstone Deck Maker)
## Introduction
For my Individual Project I am going to make a Hearthstone Deck Maker. On this web application you can get an overview over all the cards available in the game, get an overview of created decks by all users of the application and a page to create a deck yourself. For the card overview I got my inspiration from the [Hearthstone](https://hearthstone.blizzard.com/en-us/cards?set=standard&sort=dateadded%3Adesc%2Cname%3Aasc%2Cclasses%3Aasc) site.
![Hearthstone Card Overview](https://github.com/S3-HSDM/Portfolio/blob/main/images/cardoverview.jpg?raw=true)

For the deck overview I got my inspiration mainly from [HearthPwn](https://www.hearthpwn.com/decks?filter-show-standard=1&filter-show-constructed-only=y&filter-deck-tag=1) site.
![HearthPwn Deck Overview](https://github.com/S3-HSDM/Portfolio/blob/main/images/deckoverview.jpg?raw=true)

## Project choices
For this project I work according to the Agile ideology. I do this by working with Kanban method. Therefor I created a Kanban board on [Github](https://github.com/orgs/S3-HSDM/projects/1). The reason to choose for Kanban come from research I have done towards [Agile](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Agile.md) working. The languages and frameworks I use for my Individual Project are Java Spring Boot for the Backand of the project and Javascript Angular for the Frontend. The reasoning for choosing these languages/frameworks are further explained in my research files. [Backend](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Java%20Backend%20Research.md) & [Frontend](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Javascript%20Frontend%20Research.md)

## Software design
Before I could start coding for my web application I made Requirements, functional and non-functional. With those requirements I created user stories for my project. After the user stories I created a C4-model for my project. Those user stories and diagrams can be found in my documentation files. [Analysis Document](https://github.com/S3-HSDM/Portfolio/blob/main/Research%20%26%20Documentation/Documentation.md)

## Learning Outcomes (LO)
For this semester we have to match some learning outcomes. These learning outcomes are displayed [here](https://github.com/S3-HSDM/Portfolio/blob/main/Learning%20Outcomes.md).

## CI/CD (LO-4)
### CI
To ensure that my project on the main branche is a working version I added CI via Github Actions. Everytime something is pushed to the main branch, via a pull request from the development branch, the Github action runs all the tests and Sonarcloud. For my Backend it runs a serie of Unittests, Integrationtests and Regressiontest. For the Frontend it runs Unittest and Regressiontests.

![Backend Github Actions](https://github.com/S3-HSDM/Portfolio/blob/main/images/BackendActions.png?raw=true)
The tests running in the backend can be seen [here](https://github.com/S3-HSDM/HSDM-BackEnd/tree/main/hsdm/src/test/java/nl/fhict/s3/hsdm). The folders contain the unittests and the HSDMApplicationTests.java file contains the Integrationtests.
![Frontend Github Actions](https://github.com/S3-HSDM/Portfolio/blob/main/images/FrontendActions.png?raw=true)

### CD
For CD I setted up Docker for my project. Via a Docker-compose file 4 containers are created, one for my Frontend, one for my Backend and two to set up the Database. With those containers running my project runs on localhost. With the Docker images of my project, anyone can run my project on any device.

![Docker Containers](https://github.com/S3-HSDM/Portfolio/blob/main/images/Docker.png?raw=true)
