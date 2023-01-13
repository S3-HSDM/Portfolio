# Learning Outcomes & Reflection
1. You design and build **user-friendly**, **full-stack** web applications. 
   - User-friendly: You apply basic User experience testing and development techniques.
   - Full-stack: You design and build a full stack application using commonly accepted front end (Javascript-based framework) and back end techniques (e.g. Object Relational Mapping) choosing and implementing relevant communication protocols and addressing asynchronous communication issues.

For my IP I've created a full-stack webapplication with a fully functional cards CRUD operation in which normal users only have the Read functionality for cards and admin can Create, Read, Update and Delete the cards. I've created the Frontend in a Javascript framework, Angular and the Backend in a Java framework Spring Boot. For the GP I've created the Jumbo Scraper functionality, further I've created the (Retailer)NotFound pages and set up the routing for the pages in the Frontend. In the Backend I've created the create product endpoint. These contributions I'd say the score for Learning Outcome 1 is Proficient.

2. You use software **tooling and methodology** that continuously monitors and improve the software quality during software development. 
   - Tooling and methodology: Carry out, monitor and report on unit integration, regression and system tests, with attention for security and performance aspects, as well as applying static code analysis and code reviews.

To ensure the Software Quality I've created Unittests for my Backend and Frontend. Also I've set up Endpoint test for the Backend with the use of Postman. I've also added Sonarcloud to the CI pipeline for my project. With the help of Sonarcloud of bettered the Software Quality of my project by fixing the Bugs, Vulnerabilities, Code Smells, Security Hotspots and Duplications. </br>
Also I've run performance tests on my application in the form of Lighthouse. With the help of Lighthouse I've upped my Lighthouse Performance score from 36 to 68, massively reducing the loading times of my pages. </br>
Further I've done a security test for Cross-site Scripting (XSS). I've tested all my input boxes with common XSS commands. </br>
I've also implemented Auth0 to create a secure Authentication for my application.
I think doing these things lead to a score of Proficient for Learning Outcome 2.

3. You **choose** and implement the most suitable agile software development method for your software project.
   - Choose: 	You are aware of the most popular agile methods and their underlying agile principles. Your choice of a method is motivated and based on well-defined selection criteria and context analyses.

I've followed a workshop and I've done research towards Agile and different methods to work Agile. For my IP I've followed the Kanban method and created a Kanban board to keep track of my Tasks and User Stories. In the GP I've worked according to the Scrum method. We had sprints lasting 3 weeks and on the project days we had stand-up meeting to start the day. During these stand-up meetings we used our Scrumboard to check on open issues for our project and keep check of the progress. Making use of the Agile working methods I would say my score would be Proficient for Learning Outcome 3.

4. You **design and implement** a (semi)automated software release process that matches the needs of the project context.
   - Design and implement: You design a release process and implement a continuous integration and deployment solution (using e.g. Gitlab CI and Docker).

For Learning Outcome 4 I've set up a CI pipeline for my Frontend and Backend. Those CI pipelines runs everytime new code is added to main branch, running the tests I've created for my project and the Sonarcloud scans. I've also set up a Docker-compose file, which create 4 Docker Containers from my project. 1 for my Frontend, 1 for my Backend and 2 for my Database(MySQL and PHPMyAdmin). In my opinion setting up the CI/CD in this way would lead to a Proficient score for Learning Outcome 4.

5. You **recognize** and **take into account** cultural differences between project stakeholders and ethical aspects in software development.
   - Recognize: Recognition is based on theoretically substantiated awareness of cultural differences and ethical aspects in software engineering.
   - Take into account: Adapt your communication, working, and behavior styles to reflect project stakeholders from different cultures; Address one of the standard Programming Ethical Guidelines (e.g., ACM Code of Ethics and Professional Conduct) in your work.

For Cultural Differences and Ethics I've done a research towards these subject. With these researches in mind I've evaluated my own project for ethical issues and thought about what I would do different in future projects keeping the ethical principles in mind. Doing this research and evaluating my own project would in my opinion lead to a Proficient score for Learning Outcome 5.

6. You analyze (non-functional) requirements, elaborate (architectural) designs and validate them using **multiple types of test techniques**.
   - Multiple types of test techniques: You apply user acceptance testing and stakeholder feedback to validate the quality of the requirements. You evaluate the quality of the design (e.g., by testing or prototyping) taking into account the formulated quality properties like security and performance.

For my IP I've created (non-functional) requirements and discussed those with the stakeholder. With those requirements I've set up User stories. After this I create my architecture design with the help of a C4-model. For our GP after we got our assignment we set up the requirements and user stories for our group project. Together with the design wireframes we discussed these with the stakeholder to ensure we build the right thing and we discussed the importance of the requirements to decide the order of implementing the requirements. In my opinion doing these things lead to a Proficient score for Learning Outcome 6.

7. You analyze and describe **simple** business processes that are **related** to your project.
   - Simple:Involving stakeholders, predominantly sequential processes with one or two alternative paths.
   - Related:Business processes during which the software that you are developing will be used (business processes that the software must support by fully or partially automating them). **or** Business processes needed for the success of your software development project (e.g., product release, market release, financial assurance).

For business processes I've followed a workshop and researched what a business process is. After gathering knowledge about this topic I've analysed the business process our GP automates. I've analysed how our project infected/changed the business process and people who are part of the business process. I think the analysis and visualisation I've made about the business process lead to a score of Proficient for Learning Outcome 7.

8. You act in a **professional manner** during software development and learning.
   - Professional manner: You actively ask and apply feedback from stakeholders and advise them on the most optimal technical and design (architectural) solutions. You choose and substantiate solutions for a given problem.

In my IP I've had weekly meet-ups with the stakeholder, in which I first discussed my requirements and software design. Later I showed demo's about the newly implemented features. With the feedback from the stakeholder I changed the path I wanted to create my project. I wanted to keep implementing features and creating a fancier design, but the stakeholder gave the feedback to think about the quality instead of the quantity of my features, which made me realise I also had to take care of testing the features. </br>
In our GP we had 3 week lasting sprints. At the end of each sprint we had a delivery. The first sprint we used to make sure we build the right thing. We did this with the use of our requirements, user stories and wireframes and discussed those with the stakeholder. With the feedback we changed our requirements and design. After each sprint we had a sprint review in which we discussed what went well that sprint and what could go better. During the meet-ups we also agreed with the stakeholder what were going to do for the next sprint. </br>
These points In my opinion lead to a score of Proficient for Learning Outcome 8.

# Reflection
Having the weekly meet ups with the teacher helped me a lot to keep track of what I had to do during the semester. Not in terms of what had to be done in the project, but to keep track of all my learning outcomes and not forget about those. Als I liked the weekly meet ups, since I normally hold back in asking feedback talks, because at some moments I feel like I made not enough progress to discuss stuff with the teacher. This time the weekly meetings were planned, so for future projects it could be a good idea to plan fixed moments to force myself to ask for feedback and discuss the next steps in the project. </br>
Another point I could do better in the future is keeping track of my task board. When working on bigger tasks, which I already should split up more in smaller pieces, I tend to lose focus on the task board. When I'm busy on a bigger task and I already know what I can do that day and tend to neglect the task board, which becomes outdated because of that. For future projects I want to split up tasks more so I have to use my task board more. In our Group Project the use of our Task board went better. During our stand ups we used our task board to keep progress of the open tasks/issues.

I'm proud of the application I've created, even though I've could implement less features than I hoped for/came up with in the beginning. But I'm still proud of the features I have been able to implement, since I've had to learn a lot of new technologies and processes. Java Spring Boot I had used before, but I had never used inheritance before. It was also the first time I worked with Angular, which I really liked. The fact that Angular splits the Javascript/Typescript from the HTML page helps me a lot to keep track of the pages I'm making. </br>
Also setting up the CI/CD was a process I had not set up before. Especially setting up the Docker container for the Java Backend satisfied me since I struggled a lot with creating the Dockerfile, which needed a project.jar file, which at first I couldn't figure where to find or how to create that file. Also setting up the Docker container for the frontend took me longer, because starting up the container took longer than I expected. I checked if the container was running to early, which led to an error saying localhost didn't receive any data. After trying another time I found out it took Docker longer to start the frontend then it did locally. </br>
Setting up the CI pipeline for automating my tests and running Sonarcloud is another thing I've learned this semester. Creating workflow files in Github was something I had not done before. Also it was the first time I made use of Sonarcloud, but it's definitely a tool I want to keep using in the future. It's a easy to use tool to check your existing code and new code for improving clean code.
