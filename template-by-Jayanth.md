# INVEST Principle for User Stories

When you write user stories, I want you to follow the **INVEST principle**. It’s a simple checklist to make sure your stories are clear, useful, and easy to work with.

* **I** – Independent
* **N** – Negotiable
* **V** – Valuable
* **E** – Estimable
* **S** – Small
* **T** – Testable

---

## 1. Independent

Each story should stand on its own and not depend too heavily on others.

For example, in the sample:

* *Login* is separate from *Collect Coins*

What I don’t want:

> “As a player, I want to collect coins after logging in and completing a level…”

This mixes multiple features together.

Instead, split them like we did:

* Login
* Collect Coins

---

## 2. Negotiable

Your story is not a strict contract—it’s a starting point for discussion.

For example:

* “I want to log into my account” doesn’t specify how (email, Google login, etc.)

That’s intentional.

Don’t over-specify the solution in the story itself. We’ll figure out the details together.

---

## 3. Valuable

Every story must deliver clear value to the player.

Examples:

* Login → access progress and play the game
* Collect Coins → increase score and purchase upgrades

If your “So that…” part is weak or missing, the story isn’t good enough.

Bad example:

> “I want a login button” ❌

---

## 4. Estimable

I should be able to roughly estimate how much effort your story will take.

Good examples:

* Login
* Collect Coins

Bad example:

> “I want a complete multiplayer system” ❌

That’s too vague and too big. Break it down.

---

## 5. Small

Stories should be small enough to complete in a short time (a few days).

Good:

* Login
* Collect Coins

Too big:

> “I want a full inventory and shop system” ❌

Better:

* View inventory
* Add item to inventory
* Purchase item from shop

---

## 6. Testable

I should be able to clearly verify when your story is done.

This is why your **Acceptance Criteria** matter.

Examples:

* Given valid credentials → user logs in
* Given invalid credentials → error is shown
* When player touches coin → score increases

If you can’t write clear **Given / When / Then**, your story isn’t ready.

---

## Final Reminder

When you write stories, make sure they are:

* Focused and not mixed together
* Open for discussion
* Clearly valuable to the player
* Easy to estimate
* Small enough to complete quickly
* Testable with clear acceptance criteria

If your story doesn’t meet these, refine it before moving forward.