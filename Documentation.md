# Documentation
# Documentation
<h1> ANALYSIS <h1/>
<h2> Requirements <h2/>
<h3> Functional requirements <h3/>
<h4> MUST: <h4/>
<p>
FR-1.	An user has to be able to create an account. <br/>
       B-1.1	An username has to be unique. <br/>
       B-1.2	A password has to match the safety requirements. <br/>
       B-1.3	An e-mail address has to be unique. <br/>
FR-2.	An user has to be able to log in. <br/>
FR-3.	An user has to be able to change his credentials. <br/>
       K-3.1	Username, password and e-mail address has to be changeable. <br/>
FR-4.	An user can add decks. <br/>
       K-4.1	The decks will be available to all users. <br/>
       B-4.2	A deck has to contain 30 cards. <br/>
       B-4.3	A deck can’t contain more than 2 copies of the same card. <br/>
       B-4.4	A deck has an unique name. <br/>
FR-5.	An user can manage his decks <br/>
       K-5.1	Save, Edit & Delete <br/>
FR-6.	An user has to be able to view all available cards. <br/>
       B-6.1	The cards can be filtered on Cost, Rarity, Type, Set & Class of the card. <br/>
       K-Alg-1.	If something is entered wrong, the user has to get an visual error message. <br/> 
<p/>
<br/>
<h4> SHOULD: <h4/>
---
<p>
FR-7.	An user should be able to see all decks shared on the web application. <br/>
       B-7.1	Decks can be filtered based on Class. <br/>
       B-7.2	Decks can be filtered based on cards that it should(n’t) contain. <br/>
       K-7.1	An user should be able to copy and edit the copied deck for his own use. <br/>
<p/>
 <br/>
<h4> COULD: <h4/>
---
<p>
FR-8.	An user could also create ‘Wild’ & ‘Classic’ decks. <br/>
<p/>
 <br/>
<h4> WON’T: <h4/>
---
<p>
FR-9.	Decks for ‘Duel’ won’t be available. <br/>
FR-10.	Cards for ‘Battlegrounds’ and ‘Mercenaries’ won’t be available. <br/>
<p/>
<br/>
<h3> Non-functional requirements <h3/>
---
<p>
NFR 1.	The web application has to be easy to use for the users <br/>
NFR 2.	The web application has to be loaded within 10 seconds <br/>
NFR 2.1	The aim will be within 2 seconds <br/>
<p/>
<br/>
<h2> User Stories <h2/>
---
<p>
1.	As an user I want to be able to create an account, so I can create decks. <br/>
2.	As an user I want to be able to log in, so I can access my decks. <br/>
3.	As an user I want to be able to see and filter other shared decks, so I can learn new deck and get inspiration to create other decks. <br/>
4.	As an user I want to be able to see and filter all available cards, so I can compare similar cards or find all cards of the same type. <br/>
5.	As an user I want to be able to manage my decks, so when a deck becomes less relevant, I could edit or delete the deck. <br/>
6.	As an admin I want to be able to change credentials of users and decks, so the names won’t be inappropriate. <br/>
7.	As an admin I want to be able to manage the cards, so the web application has all the cards that are available. <br/>
<p/>
