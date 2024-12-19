# User Stories


📘  Our service receives requests from a client that includes the query param `isAdmin=true` or `isAdmin=false`

- As an Admin user, I should see the first and last names of all players. 
- As a regular user, I should only see the first names of all players. 

Scope:

- Plan and implement a new feature in your service
- Add test coverage

---

📘  As a User, when I make a request to `/v1/players` or `v1/players/{id}`, I would like to see the players' ages in the response. 

Scope:

- Plan and implement given feature in your service.
- Add test coverage. 

---

📘  As a developer, I would like to improve the performance of `getPlayerById` API  which is subpar and is causing slow load times on the front end. (Note: You may not remove the simulated delay added in the code)

---

📘  As a developer, I would like to have test cases written out for implemented utility functions

---

📘  Our service needs to store the following information for players: 

- Managers
- Teams
- Batting
- Fielding
- Pitching
    
Discuss how you would design your database to support these data dependencies.

---

📘  Our team has been tasked with supporting the creation of any sport and its players. The player attributes may change for each sport. What type of considerations would you propose to the team? 

---

📙 **AI Story**:  As a User, I'd like to generate a player nickname based on a given country. 

Scope:
- Leverage provided LLM to generate nickname
- Leverage given model (tinyllama) to implement the functionality under CHAT mode by making use of SYSTEM & USER prompts
- Create a new API to wrap this functionality
- Create the output either in text/valid JSON as part of this API
- Add 1 unit test : variate the prompt to test few scenarios
- Dataset assumptions (Pick one of these options) 
       1. Pickup data from Player.csv 
       2. Pickup examples from google

---

📙 **AI Story**:  As a User, I'd like to recommend a list of players for a tournament based on sample features such as demographic, matches they played, etc
Scope:
- Leverage LLM model provided to generate recommendation of list of players for a tournament given features from dataset
- Select a few features from the Player.csv and send the data to genAI model
- Leverage given model to implement the functionality under CHAT mode by making use of SYSTEM & USER prompts
- Create a new API to wrap this functionality
- Create the output either in text/valid JSON as part of this API
- Add 1 unit test : variate the prompt to test few scenarios
- Add guardrails to avoid hallucinations

---

📙 **AI Story**:  As a User, I'd like to recommend a list of players for a tournament based on sample features such as demographic, matches they played, etc

Scope:
- Leverage the provided AI service (player-service) to generate recommendation of list of players for a tournament given features from the dataset OR a player from the dataset as a seed
- Create a new API to wrap this functionality.
- Create the output either in text/valid JSON as part of this API
- Add 1 unit test : validate input/output to test few scenarios
- Add guardrails to avoid out of bounds data

---

