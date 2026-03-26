# Login

## Story 1:

As a player<br>
I want to log into my account<br>
So that I can access my progress and play the game

### Acceptance criteria

* **Given** I am on the login screen<br>
  **When** I enter a valid username and password<br>
  **Then** I am successfully logged in and taken to the main menu

* **Given** I am on the login screen<br>
  **When** I enter an incorrect username or password<br>
  **Then** I see an error message indicating invalid credentials

* **Given** I am on the login screen<br>
  **When** I leave the username or password field empty and try to login<br>
  **Then** I see a validation message prompting me to fill in the required fields<br>

* **Given** I am logged in<br>
  **When** I relaunch the game within a short session period<br>
  **Then** I remain logged in and do not need to enter credentials again

---

# Main-menu

## Story 1:

As a player<br>
I want to host a game<br>
So that I can play with my friends

### Acceptance criteria

* **Given** I am on the main-menu<br>
  **When** I select host game option<br>
  **Then** I move to waiting lobby with a room-id

## Story 2:

As a player<br>
I want to join a game<br>
So that I can play with my friends

### Acceptance criteria

* **Given** I am on the main-menu<br>
  **When** I select join game option<br>
  **Then** I get asked for room-id

* **Given** I select join game option<br>
  **When** I enter a valid room-id<br>
  **Then** I move to waiting room with a room-id

* **Given** I select join game option<br>
  **When** I enter an invalid room-id<br>
  **Then** I see an error message indicating invalid room-id

* **Given** I select join game option<br>
  **When** I leave the username or room-id field empty and try to enter<br>
  **Then** I see a validation message prompting me to fill in the required fields<br>

* **Given** I select join game option<br>
  **When** No games are hosted<br>
  **Then** I see a prompt indicating no rooms are hosted

* **Given** I select join game option<br>
  **When** I enter a valid room-id that is full<br>
  **Then** I see a prompt indicating room full<br>

## Story 3:

As a player<br>
I want to know the rules and description of the game<br>
So that I can play the game appropiately

### Acceptance criteria

* **Given** I am on the main-menu<br>
  **When** I select about game option<br>
  **Then** I see rules and description of the game

# Lobby-management

## Story 1: View players in lobby

As a player<br>
I want to see who has joined the lobby<br>
So that I know who I will be playing with

### Acceptance Criteria

* **Given** I am in the waiting lobby<br>
* **When** players join or leave<br>
* **Then** I see the updated list of players in real-time<br>

* **Given** I am in the waiting lobby<br>
* **When** I view the player list<br>
* **Then** I see player names and host indication<br>

## Story 2: Start game (Host only)

As a host<br>
I want to start the game<br>
So that gameplay can begin when all players are ready

### Acceptance criteria

* **Given** I am the host in the lobby<br>
* **When** minimum required players have joined<br>
* **Then** I can see the "Start Game" button enabled

* **Given** I am the host<br>
* **When** I click "Start Game"<br>
* **Then** all players are moved to game setup

* **Given** I am not the host<br>
* **When** I am in the lobby<br>
* **Then** I cannot start the game

## Story 3: Leave lobby

As a player<br>
I want to leave the lobby<br>
So that I can exit the current game session

### Acceptance criteria

* **Given** I am in a lobby<br>
* **When** I select leave lobby<br>
* **Then** I return to main menu

* **Given** I am the host and leave<br>
* **When** I exit the lobby<br>
* **Then** host privileges are transferred or lobby is closed

# Game-setup

## Story 1:

As a player
I want the setup
So that I can start to play the game

### Acceptance criteria

* **Given** I am in the game room<br>
  **When** Organ cards are dealt evenly and 5 attack cards dealt to each player<br>
  **Then** I should see all players organ card and my attack cards

* **Given** Cards are dealt<br>
  **When** I see all players organ card and my attack cards<br>
  **Then** Player with the wild organ gets the first turn

---
