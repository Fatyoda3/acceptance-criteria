# Stories

## Login

As a player
I want to log into my account
So that I can access my progress and play the game

### Acceptance criteria

* **Given** I am on the login screen
  **When** I enter a valid username and password
  **Then** I am successfully logged in and taken to the main menu

* **Given** I am on the login screen
  **When** I enter an incorrect username or password
  **Then** I see an error message indicating invalid credentials

* **Given** I am on the login screen
  **When** I leave the username or password field empty and try to log in
  **Then** I see a validation message prompting me to fill in the required fields

* **Given** I am logged in
  **When** I relaunch the game within a short session period
  **Then** I remain logged in and do not need to enter credentials again

---

## Collect Coins

As a player
I want to collect coins during gameplay
So that I can increase my score and purchase upgrades

### Acceptance criteria

* **Given** I am playing a level
  **When** my character touches a coin
  **Then** the coin is collected and my score increases

* **Given** I collect a coin
  **When** the coin is added to my total
  **Then** I see visual and/or audio feedback confirming the collection

* **Given** I finish a level
  **When** coins were collected during gameplay
  **Then** the total coins are added to my overall balance

* **Given** I have enough coins
  **When** I visit the in-game shop
  **Then** I can spend coins to purchase available upgrades
