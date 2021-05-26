# group-2-project-2
Revature2103 Reactive Java, Group 2 Project 2

# Project Description
Project 2 is a Deck Building API where the main objective is to create a datebase of cards created by the owner of the server.  The API allows to add or remove cards for the owner for other users to collect and edit their decks with the cards they own.  The users can also exchange their cards with other users based on posting a trade request.  

# Technologies Used
- Java
- Spring
- NoSQL
- REST
- JUnit
- Log4J
- Mockito
- Postman
- AWS Keyspace

# Roles / Responsibilities:
-	Created the process of approval among the Department Head, Direct Supervisor, and Benefit Coordinator
-	Created Keyspaces in AWS to store information of users and Tuition Reimbursement forms
-	Implemented Admin’s ability to approve or disapprove forms from users.
-	Used junit testing to provide information if functions in the program are operating as attended.
-	Ensure the ordering of the approval process is set in order.
-	Calculate the formula of the reimbursement system.
-	Created types of their reimbursement coverage based on what course the user took.
-	Created a system to automatically approve reimbursement if deadline is met late.


# Features
-	Allow to create cards within the system (Admin only).
-	Allow to collect cards that are in the database.
-	Allow to trade cards with other users within the system.
-	
# To-do list:
- Allow the admins to upload more then one card at a time.
- Allow users to battle each other.

# Getting Started
1.	Install Git Bash (https://git-scm.com/downloads), and Eclipse (https://www.eclipse.org/downloads/) onto your computer.
2.	Launch your Git Bash application and input the following commands:
a.	Git clone https://github.com/rnbiv45/group-2-project-2
b.	Cd rBowmanProject1
c.	Git pull origin main
3.	Launch the group-2-project-2 application.

# Usage
With postman, you will be able to send commands to the Deck Building API as follows:
- http://localhost:8080
- POST /users/register: Register as a user using body as an input (“name”: (input name), “pass”: (input password)
- POST /users/login: Login as a user using body as input (“name”: (input name), “pass”: (input password)
- DELETE /users/logout: Logout as user.
- GET /users: View all users in the system.
- GET /decks: View all decks in the system.
- POST /decks: Add card in the deck with form data taking a card’s ID the user has (“cardUuid” : (card’s id)
- GET /decks/user: View decks the user logged in has.
- POST /decks: Create a deck using primaryArchetypes and secondaryArchetype as a form data.  Choose between, Fire, Earth, Wind, or Water.  (“primaryArchetypes”: (Fire, Earth, Wind, or Water) “secondaryArchetype”: (Fire, Earth, Wind, or Water))
- POST /cards: Add card to the system by setting up the body with the following types: 
- POST /cards/new/(card name here): Add card to the collection of the logged in user
- PUT /cards: Change the cards stats base on name, isUnique, attackValue, defenseValue, damageValue, and/or buffValue.  Use Id of the card to pick which card to change.
- GET /cards: View all cards in the system.
- GET /cards?type=(choose type): View all cards based on it’s type
- GET /trade: View all the pending trades.  This will allow the user to see pending trades to trade different cards
- POST /trade/submit: Pick 1 card the user is willing to trade, and 1 card the user wishes to have with the trade based on ID.
- POST /trade/accept: Pick the ID of the trade to exchange the card with the trader.

# Contributors
- Robert Bierly
- Nerijus Gelezinis
- AlbertMagpoc

# License
This project uses the following license: 

