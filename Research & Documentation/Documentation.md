# Documentation
## Requirements
### Functional requirements

**MUST:**
1.  An user has to be able to create an account.
    - B-1.1	An username has to be unique.
    - B-1.2	A password has to match the safety requirements.
    - B-1.3	An e-mail address has to be unique.
2.  An user has to be able to log in.
3.  An user has to be able to change his credentials.
    - K-3.1	Username, password and e-mail address has to be changeable.
4.  An user can add decks.
    - K-4.1	The decks will be available to all users.
    - B-4.2	A deck has to contain 30 cards.
    - B-4.3	A deck can’t contain more than 2 copies of the same card.
    - B-4.4	A deck has an unique name.
5.  An user can manage his decks.
    - K-5.1	Save, Edit & Delete.
6.  An user has to be able to view all available cards.
    - B-6.1	The cards can be filtered on Cost, Rarity, Type, Set & Class of the card.
    - K-Alg-1.	If something is entered wrong, the user has to get an visual error message.

**SHOULD:**

7.  An user should be able to see all decks shared on the web application.
    - B-7.1	Decks can be filtered based on Class.
    - B-7.2	Decks can be filtered based on cards that it should(n’t) contain.
    - K-7.1	An user should be able to copy and edit the copied deck for his own use.

**COULD:**

8.  An user could also create ‘Wild’ & ‘Classic’ decks. 

**WON’T:**

9.	 Decks for ‘Duel’ won’t be available.
10. Cards for ‘Battlegrounds’ and ‘Mercenaries’ won’t be available.

### Non-functional requirements
1. The web application has to be easy to use for the users.
2. The web application has to be loaded within 10 seconds.
   - 2.1 The aim will be within 2 seconds.
### User Stories 
1.	As an user I want to be able to create an account, so I can create decks.
2.	As an user I want to be able to log in, so I can access my decks.
3.	As an user I want to be able to see and filter other shared decks, so I can learn new deck and get inspiration to create other decks.
4.	As an user I want to be able to see and filter all available cards, so I can compare similar cards or find all cards of the same type.
5.	As an user I want to be able to manage my decks, so when a deck becomes less relevant, I could edit or delete the deck.
6.	As an admin I want to be able to change credentials of users and decks, so the names won’t be inappropriate.
7.	As an admin I want to be able to manage the cards, so the web application has all the cards that are available.