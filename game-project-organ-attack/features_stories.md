# Login

## Story 1: Login

As a player<br>
I want to log into my account<br>
So that I can access my progress and play the game

### Acceptance criteria

* **Given** I am on the login screen<br>
  **When** I enter a valid username and password<br>
  **Then** I am successfully logged in and taken to the main menu
---
* **Given** I am on the login screen<br>
  **When** I enter an incorrect username or password<br>
  **Then** I see an error message indicating invalid credentials
---
* **Given** I am on the login screen<br>
  **When** I leave the username or password field empty and try to login<br>
  **Then** I see a validation message prompting me to fill in the required fields<br>
---
* **Given** I am logged in<br>
  **When** I relaunch the game within a short  period of time  after exiting the earlier the game page<br>
  **Then** I remain logged in and my credentials must persist 
---
## Story 2: Logout

As a player<br>
I want to log out<br>
So that I can securely exit my account

### Acceptance Criteria

* **Given** I am logged in<br>
* **When** I select logout<br>
* **Then** I am logged out and redirected to login screen
---

# Main-menu
## Story 1a: Profile Icon
  As a logged in player<br>
  I want to see my profile icon and username<br>
  So that I can confirm my username and share with other players 

## Story 1b: Host game

As a logged in player<br>
I want to host a game<br>
So that I can create a session for others to join

### Acceptance criteria
---
* **Given** I am on the main-menu<br>
* **When** I select host game option<br>
* **Then** Then I am taken to a lobby with a generated room ID

---

## Story 2: Join game

As a logged in player<br>
I want to join a game<br>
So that I can play with others

### Acceptance criteria

* **Given** I am on the main-menu<br>
  **When** I select join game option<br>
  **Then** I am prompted to enter a room ID
---
* **Given** I enter a valid room ID<br>
* **When** I submit<br>
* **Then** I join the corresponding lobby
---
* **Given** I enter an invalid room ID<br>
* **When** I submit<br>
* **Then** I see an error message
---
* **Given** I leave the room ID field empty<br>
* **When** I try to join<br>
* **Then** I see a validation message prompting me to fill in the required fields<br>
---
* **Given** no active rooms exist<br>
  **When** I try to join<br>
  **Then** I see a prompt indicating "no rooms are hosted try hosting room"
---
* **Given** I enter a valid room-id that is full<br>
  **When** I try to join the room <br>
  **Then** I see a prompt indicating room full, host or try another room <br>
---
## Story 3: About game and rules

As a logged in player<br>
I want to know the rules and description of the game<br>
So that I can play the game appropriately

### Acceptance criteria

* **Given** I am on the main-menu<br>
  **When** I select about the game option<br>
  **Then** I see the rules and description of the game
---

* **Given** I am in a game session<br>
  **When** I want to refer some rule <br>
  **Then** I should see be able to see the rules and game description of the game
--- 
#  Lobby-management

## Story 1: View players in lobby

As a player<br>
I want to see who has joined the lobby<br>
So that I know who I will be playing with

### Acceptance Criteria

* **Given** I am in the waiting lobby<br>
* **When** players join or leave<br>
* **Then** I see the updated list of players in real-time<br>
---
* **Given** I am in the waiting lobby<br>
* **When** I view the player list<br>
* **Then** I see player names and host indication<br>
---
* **Given** I am in the waiting lobby<br>
* **When** Game is not started<br>
* **Then** I should see waiting for other players
--- 
* **Given** I am in the waiting lobby<br>
* **When** a player joins <br>
* **Then** I should see updated player count
--- 
* **Given** I am in the waiting lobby<br>
* **When** I waited for too long <br>
* **Then** I should be able to leave the current lobby
--- 
* **Given** I left the waiting lobby<br>
* **When** I should go back to home screen
* **Then** I should be able to navigate to join or create or logout

## Story 2: Start game (Host only)

As a host<br>
I want to start the game<br>
So that gameplay can begin when all players are ready

### Acceptance criteria

* **Given** I am the host in the lobby<br>
* **When** minimum required players have joined<br>
* **Then** I can see the "Start Game" button enabled
---
* **Given** I am the host<br>
* **When** I click "Start Game"<br>
* **Then** all players are moved to game setup
---
* **Given** I am not the host<br>
* **When** I am in the lobby<br>
* **Then** I cannot start the game

## Story 3: Leave lobby

As a player<br>
I want to leave the lobby<br>
So that I can exit the current game session

### Acceptance criteria
---
* **Given** I am the host<br>
* **When** I leave the room<br>
* **Then** the room is removed and everyone leaves
---

* **Given** I am in a lobby<br>
* **When** I select leave lobby<br>
* **Then** I return to main menu
---
* **Given** I am the host and leave<br>
* **When** I exit the lobby<br>
* **Then** host privileges are transferred or lobby is closed

# Game-setup

## Story 1: Card Distribution

As a player<br>
I want to receive<br> 
So that I can begin gameplay

### Acceptance criteria

* **Given** I am in the game room<br>
  **When** Organ cards are dealt evenly<br>
  **Then** I should see all other players organ card 
---
* **Given** I am in the game room<br>
  **When**  5 attack cards dealt to each player<br>
  **Then** I should see my attack cards 
---
* **Given** I am in the game room<br>
  **When** cards are dealt <br>
  **Then** player with the wild organ gets the first turn
---
* **Given** cards are dealt <br>
  **When** player with the wild organ is identified<br>
  **Then**game starts 
---

# Player turn

# Afflictions
---

- ## Story 1: normal affliction

As a player<br>
I want to play normal affliction card on an opponent with the organ mentioned on the card<br>
So that I can afflict chosen opponent's specific organ mentioned on the card

### Acceptance criteria

* **Given** I play the card<br>
* **When**It is not blocked<br>
* **Then** Opponents organ will sustain damage 
---
* **Given** I play the card <br>
*  **When**It is blocked<br>
*  **Then** Opponents organ will sustain no damage, 
---
* **Given** opponent has vaccine  <br>
*  **When** I play the card<br>
*  **Then** Opponents organ will sustain no damage, and the vaccine will lose a point
---

- ## Story 2: remove affliction 

As a player<br>
I want to play remove affliction card on an opponent with the organ mentioned on the card<br>
So that I can remove chosen opponent's specific organ mentioned on the card

- ## Story 3: Hybrid affliction

As a player<br>
I want to play hybrid affliction card on an opponent with the organ mentioned on the card<br>
So that I can choose to remove or afflict chosen opponent' specific organ mentioned on the card

- ## Story 4: Wild affliction

As a player<br>
I want to play wild affliction card on any opponent<br>
So that I afflict any organ of my choice of the chosen opponent

- ## Story 5: Necrosis

As a player<br>
I want to play necrosis card on any opponent<br>
So that I remove any organ of my choice of the chosen opponent

- ## Story 5: Contagious

As an attacked player<br>
I want to play contagious card on the any opponent<br>
So that I afflict their organ of my choice of the chosen opponent

- ## Story 6: Metastasis

As a attacking player<br>
I want to play metastasis card on the same opponent, whom i played an affliction on<br>
So that I afflict another organ of my choice of the opponent

- # Cure

    - ## Story 1: Medicine

    As an already afflicted player<br>
    I want to play medicine card on one of my afflicted organ<br>
    So that I can increase the health of the chosen organ by 1

  - ## Story 2: Medical miracle

    As an already afflicted player<br>
    I want to play medical miracle card on one or two of my afflicted organ(s)<br>
    So that I can increase the health of the chosen organ(s) by 1/2 

- # Sleep

    - ## Story 1: Sedate

    As a player<br>
    I want to play sedate card on any opponent<br>
    So that I can make them sleep and skip their turns for the next 2 turns

    - ## Story 2: Narcolepsy

    As a player<br>
    I want to play narcolepsy card on any opponent<br>
    So that I can make them sleep and skip their next turn

- # Bureaucracy

    - ## Story 1: Research

    As a player<br>
    I want to play research card<br>
    So that I can take a card from the discard pile of my choice

    - ## Story 2: Clinical audit

    As a player<br>
    I want to play clinical audit card<br>
    So that I can discard a card of my choice from each opponent's hand

    - ## Story 3: By the book

    As a player<br>
    I want to play the by the book card<br>
    So that I can make every player including myself to discard all non-normal-affliction cards

- # One-time playable cards

    - ## Story 1: It's alive

    As a player who lost an organ(s)<br>
    I want to play it's alive card<br>
    So that I can reanimate a lost organ card of mine according to my choice

    - ## Story 2: Transplant

    As a player<br>
    I want to play transplant card<br>
    So that I can take any one organ card from any of my one opponents according to my choice