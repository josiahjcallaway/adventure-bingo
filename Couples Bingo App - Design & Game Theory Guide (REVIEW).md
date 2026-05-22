## Core Product Vision

This is not just a bingo app.

The product is a:
- social game
- memory generator
- travel companion
- relationship ritual
- chaos engine
- procedural scavenger hunt

The purpose of the app is to:
> make ordinary outings more memorable by injecting playful tension, observation, interaction, and inside jokes into real-world experiences.

The app should encourage:
- noticing the environment
- interacting with strangers/world
- playful competition
- collaborative memories
- spontaneity

The app should NOT become:
- task management
- overly gamified optimization
- phone-centric
- mechanically repetitive

The app should inject prompts and then disappear into the background.

---

# Core Design Principles

## 1. Shared Experience First
The game exists to improve the outing itself.

The app is secondary.

Every mechanic should answer:
> “Will this create a memorable moment together?”

---

## 2. Low Friction
Interactions must be:
- fast
- obvious
- lightweight
- glanceable

Avoid:
- excessive menus
- complicated scoring
- long rule explanations

---

## 3. Emotional Peaks Matter
The best moments come from:
- tension
- surprise
- embarrassment
- sabotage
- risk
- laughter

Not from simply checking boxes.

---

## 4. Replayability Through Variability
The game must feel different every time.

Use:
- weighted randomness
- location-based packs
- hidden objectives
- combo systems
- dynamic modifiers

---

## 5. Story Generation > Winning
Winning should matter less than:
- funny moments
- chaos
- memorable interactions
- screenshots/photos
- inside jokes

---

# Core Gameplay Loop

1. Select game mode
2. Generate randomized board
3. Explore/travel/date/etc.
4. Complete squares naturally
5. Trigger benefits/penalties
6. Progress toward bingo/full board
7. Endgame event/reward
8. Save memory archive

---

# Recommended Board Composition

## Board Types

### Shared Board
- collaborative mode
- ideal for vacations/dates

### Separate Boards
- competitive mode
- introduces sabotage/game theory

---

## Square Distribution

| Square Type | Target % | Purpose |
|---|---|---|
| Observation | 40% | Constant progress |
| Social/Interactive | 25% | Story creation |
| Rare/High-Value | 15% | Excitement spikes |
| Benefit Squares | 10% | Momentum shifts |
| Penalty Squares | 10% | Chaos/tension |

---

# Square Categories

## 1. Observation Squares

Purpose:
- maintain momentum
- encourage awareness

Examples:
- Dog wearing clothes
- Neon sign
- Someone arguing
- Scooter rider
- Luxury car
- Broken sign
- Airport delay announcement
- Matching outfits

Characteristics:
- easy
- passive
- always available

These are the “dopamine drip” mechanics.

---

## 2. Social/Interaction Squares

Purpose:
- generate memorable stories

Examples:
- Compliment a stranger
- Ask bartender for recommendation
- Fake accent for one interaction
- Order for your partner
- Ask for off-menu item
- Dramatic movie-style selfie

Characteristics:
- active participation
- mild social risk
- memorable

These are the core memory generators.

---

## 3. Couple Dynamics Squares

Purpose:
- deepen relationship-specific humor

Examples:
- Predict partner’s order correctly
- Simultaneously say same word
- Partner catches you on phone
- Public vote settles disagreement
- One partner gets recognized

These become recurring inside jokes.

---

## 4. Rare/Event Squares

Purpose:
- create excitement spikes

Examples:
- Celebrity sighting
- Someone drops drink
- Free item from staff
- Proposal spotted
- Street performer interaction

Characteristics:
- uncommon
- high-value
- rewarding

---

# Benefits & Penalties System

## Design Philosophy

Benefits and penalties should:
- alter gameplay
- create chaos
- generate tension
- force interaction

Avoid passive mechanics.

Bad:
- “Take a sip.”

Good:
- “Swap one completed square with an incomplete square.”

---

# Benefits (Good Squares)

## Strategic Benefits
Examples:
- Freeze next penalty
- Reroll square
- Reveal hidden square
- Double next completion
- Steal square
- Immunity token

Purpose:
- create tactical decisions
- encourage planning

---

## Chaos Benefits
Examples:
- Choose next venue
- Force temporary nickname
- Partner compliments you publicly
- Assign accent challenge
- Choose next photo pose

Purpose:
- comedy
- unpredictability
- social interaction

---

# Penalties (Bad Squares)

## Design Goals

Penalties should create:
- inconvenience
- embarrassment
- commitment pressure

But should NEVER:
- ruin mood
- create real conflict
- cause financial stress
- create unsafe situations

---

## Good Penalty Examples

- No phone for 10 minutes
- Speak formally for 5 minutes
- Narrate actions dramatically
- Partner chooses next drink
- Sing responses once
- Speak in movie trailer voice

---

# Drinking Version Design

## Critical Rule

DO NOT tie every square to alcohol consumption.

Otherwise:
- pacing collapses
- intoxication spikes too early
- game ends prematurely

---

## Better Drinking Structure

### Green Squares
Social/funny/no drinking

### Yellow Squares
Small drink mechanic

### Red Squares
Chaos event

### Black Squares
Temporary global modifier

Example:
> “For 15 minutes both players must speak in pirate accents.”

---

# Hidden Objectives System

## Purpose

Introduces:
- bluffing
- manipulation
- strategy
- secret incentives

---

## Examples

- Make partner say “seriously?”
- Spot 3 hats first
- Convince partner to order dessert
- Get partner to check phone
- Make partner laugh while drinking

---

# Combo System

## Purpose

Transforms gameplay from:
- passive randomness

Into:
- strategic routing
- tactical prioritization

---

## Example Combos

| Combo | Reward |
|---|---|
| 3 observation squares | Reroll token |
| Complete corners | Immunity |
| Complete center cross | Chaos event |
| Consecutive social squares | Double points |

---

# Dynamic Systems

## Timed Challenges

Examples:
- Complete within 5 minutes
- Before food arrives
- Before leaving location

Purpose:
- urgency
- adrenaline

---

## Chain Reactions

Examples:
- Completing one square mutates nearby squares
- Penalty unlocks hidden event
- Benefits evolve future board state

Purpose:
- unpredictability
- emergent gameplay

---

## Rivalry Meter

As game progresses:
- penalties intensify
- chaos increases
- rewards improve

Purpose:
- escalating tension

---

# Content Architecture

## IMPORTANT:
DO NOT hardcode content directly into frontend logic.

Use content packs and weighted entries.

---

# Suggested Schema

```csv
id,title,category,type,difficulty,weight,tags,effect