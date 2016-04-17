# Defenders of the Rift
# Gameplay

**Defenders of the Rift** is in the pattern of a [Customizable Card Game (CCG)](https://en.wikipedia.org/w/index.php?title=Customizable_card_game).
Players bring their own specialized deck of cards to each game. These decks are constructed of cards
that are selected by the player ahead of time and should be designed to work together to maximize
strategic and thematic effect.

## 1. Guidelines

The design of this game shall be governed by a few concepts. In addition to the general concepts of [FreeCCG](https://github.com/coderkevin/freeccg), this game has the additional guidelines:

### 1.1. Simplicity in Rules

**Defenders of the Rift** should be simple to learn, but difficult to master. The basics of its ruleset should be easily explained and understood within a few minutes. The numbers used for stats should be as low as possible in order to simplify the math needed to play the game.

### 1.2. Quick Gameplay

The game should play out in an average of 20 minutes. This is to ensure the game can be played without a large time commitment. While certain strategies and game variants may take considerably more time, it should always be sought to
keep the average game time to around the 20 minute mark.

## 2. Overview

With focus on simple gameplay and tactics, the **Defenders of the Rift** should be easy to learn, but with elements of strategy that are harder to master. The Flagship CCG gameplay has only a few key elements.

## 3. Deck Selection

A common part of many CCGs is the ability to select all the cards which constitute the deck of cards used for play. Each player constructs their own deck and draws from it for each turn. At some point, the number of identical cards may be restricted to a certain amount per deck, but those rules will be determined as needed.

## 4. Cards in Hand

Each player will operate from the cards held in hand. These will be restricted to a certain number, above which will require discarding at the end of the turn. Each player will draw cards toward the beginning of their turn to replenish their hand.

## 5. Card Types

There are a few specific card types: Units, Modifiers, Actions, and Avatars. Each of these types will have multiple uses, so the categories are broad, but denote the general behavior of each card type. All cards must be played on the player’s turn except for Actions, which may be played at any time during any player’s turn. All cards have a resource cost, and will have other relevant stats and abilities. Some cards may have special unique abilities written on the card itself.

### 5.1. Units

These cards represent an entity which can stand alone on the field. Each require no other cards to exist when they are placed. Most Units will have an initial resource cost for placement, some will have a recurring resource cost that must be paid every turn.  Units can have a few purposes. They may produce resources, or provide combat abilities for defense or attack. Some units may exist solely for their special abilities.

### 5.1.1. Resource Units

Some units exist for the sole purpose of resource creation. These units typically will not have any combat ability. However, even these units will have a number of hit points and can be destroyed through normal combat. Note that some Resource Units may be suitable for combat as well.

### 5.1.2. Combat Units

Combat units are designed to either attack, defend, or both. Positioning and use of these combat units will comprise an important element of strategy for the game. Note that some Combat Units will also produce resources.

### 5.2. Modifiers

Modifiers exist to be played on a Unit. All Modifiers must target a specific unit, either your own or an opponent’s when played. It is then attached to that unit permanently and cannot be removed except through explicit means. Modifiers can exist for a few reasons, either to enhance your units (increase combat stats, provide abilities, etc.) or they can harm enemy units (decrease combat stats, cause recurring health damage, etc.)

### 5.3. Actions

Actions cause immediate effects and are then discarded. All Actions must target either a Unit or a Modifier, as specified by the card. After the Action has been resolved, it is discarded. Actions may interrupt other actions and are then resolved in a "first in, last out" order.

### 5.4. Avatar/Hero

Avatars are exactly like units, except that they have a special designation. Each player may keep one Avatar card separate from the deck for use at the beginning of each game. That Avatar card represents the player and when the Avatar is defeated, the player loses the game.

## 6. Row Formation

Units are placed in rows on the field. This becomes important tactically for melee and ranged attacks, and is significant for protecting the other units.

## 7. Turn Phases

It is important that each player take his turn with each phase in a specific order: Draw, Harvest, Upkeep, Align, Place, Attack, Discard. The order of these phases is important to gameplay for several reasons. For instance, it forces the player to think ahead when aligning their units before the attack, as there will be no opportunity to realign them after the attack before the opponent’s turn.

### 7.1. Draw

The player draws 1 card from their deck. If the player’s deck has been exhausted, they may reshuffle the discard pile into their deck again, and then draw. (Alternate: no reshuffle allowed, draw is skipped if no cards remain)

### 7.2. Harvest

For each unit capable of producing a resource, place a counter on each unit for each resource it produces. Regeneration also occurs during this phase.

### 7.3. Upkeep

If any units have a recurring resource cost, these must be paid or the unit is discarded.

### 7.4. Align

At this phase, all units on the field of play may be moved freely between rows. (Alternate: Only one row forward or back)  The player should consider his strategy for the attack phase, as well as his opponents turn thereafter.

### 7.5. Place

After the alignment phase, the player has an opportunity to place new units on the field, or add modifiers to his own or his opponent’s units.  All new units must be placed either on the backmost row or form a new backmost row. New units cannot be moved until the next turn’s alignment phase. (Alternate: This phase switches place with the Attack phase)

### 7.6. Attack

At this point, the player may initiate an attack, if they wish.

### 7.7. Discard

The player must discard cards until they have a maximum of 7 cards.  Also, any resource tokens that exceed the storage capacity of a unit must be discarded as well.

## 8. Combat

### 8.1. Melee Attacks

Melee attacks may only occur from your front row to your opponents front row.

### 8.2. Ranged Attacks

Ranged attacks target up to 2 rows ahead. This includes your rows and your opponent’s rows. e.g. A ranged unit on your second row may hit the front row of the opponent.  Or a ranged unit on your front row could hit the second row of the opponent.

### 8.3. Combined Attacks

Multiple units may combine their attacks to overcome a high dodge bonus. This is akin to flanking or distracting an opponent to let your buddy get this killing blow. Attack values may be added up and the first one to overcome the dodge bonus of the opponent deals damage. Further attackers on the same opponent deal damage as well.

## 9. Card Statistics

There are several card statistics which are important to the game. These govern the basics of combat, life, and
resources. Statistics are signified by icons with a number to the left and/or right of it.

### 9.1. Life Stats

Life Stats are signified by the ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png) icon. In general, the number to the left signifies an initial value and the number to the right signifies a recurring value.

#### 9.1.1. Unit Life Stat

 * Left value: Max Life
 * Right value: Regen (or Diminish if negative)
 * Examples:
   - 3 Life: **3** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png)
   - 4 Life, 1 Regen: **4** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png) **1**
   - 5 Life, 1 Diminish: **5** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png) **-1**

#### 9.1.2. Modifier Life Stat

 * Left value: Immediate (once only) life given or taken
 * Right value: Regen (or Diminish if negative)
 * Examples:
   - Heal unit up to 2 life immediately: **2** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png)
   - Take 2 life immediately: **-2** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png)
   - Regenerate 2 life each round: ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png) **2**
   - Drain 1 life each round: ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png) **-1**

#### 9.1.2. Action Life Stat

 * Left value: Immediate (once only) life given or taken
 * Right value: Not used (actions are immediate and cannot bestow recurring effects)
 * Examples:
   - Heal unit up to 4 life immediately: **4** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png)
   - Take 3 life immediately: **-3** ![Life](https://raw.githubusercontent.com/coderkevin/defenders-of-the-rift/master/icons/life_16.png)

