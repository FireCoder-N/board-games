# Hoards

Fueled by insatiable avarice, the dragons are relentless seekers of opulence and power. Draped in scales of formidable might, driven by an unparalleled ego, these majestic beings soar across the lands with an unwavering belief that they, supreme rulers among mortal creatures, rightfully own the world's riches.
Their lairs, formidable fortresses brimming with gleaming treasures, hidden in the most treacherous corners of the realm, stand as testaments to their insatiable desire for wealth. Within those,  dragons cultivate an aura of danger and power, guarding their amassed hoards with not just innate toughness, but also with cunning traps, magical guardians, and the ferocity that comes from the self-perception as rulers.

Venture forth, oh mighty dragons; if you dare. Get ready to embark on an epic quest for glory in pursuit of riches in this captivating board game. But beware. For your kin is canny and the bigger the treasure is, the more greedy glances it attracts. Only the most powerful dragon can be the king to reign them all. After all, you do think sharing is weakness, don't you?

Hoards is a board game for 2-4 players, playing as dragons trying to hoard treasures. To play, you only need a normal deck of cards.

## Preparations
- Remove the 4 for kings from the deck.
- Also remove n+1 random cards from the deck, where n is the number of players.
- Shuffle the deck and draw 4 cards to each player.
- Each player also gets (randomly or via selection) 1 king card. Kings are special cards with unique abilities.

|  card  |   dragon    |   characteristic  | ability | 
|:------:|:-----------:|:-----------------:|:--------|
|K of ♥  |  red dragon | covetous, arrogant| the next time you are targeted by `accumulate treasure` and the outcome of comparison is a draw, you are considered the winner of the fight. |
|K of ♦  | green dragon| cunning, devious| the next time you are targeted by `accumulate treasure` and immediately before fight, you <ins>may</ins> choose that the smaller values instead of the biggest win the round. |
|K of ♠  | blue dragon | prideful, territorial| you can't be the target of the next `accumulate treasure` action.|
|K of ♣  | black dragon|   brutal, cruel  | the next time you are targeted by `accumulate treasure`'s `loot another dragon`, if you win the comparison, you won't discard any ♣ cards.

The players are free to choose any method to select the playing order, but it is adviced to pick the first player randomly.

## Goal
Accumulate the biggest hoard among all players, i.e. achieve maximum score when the deck finishes.

### Score

For all the tricks you have hoarded calculate the base score.
#### Basce Score:

$$ base = {0.8 \times \sum values(♣) + \sum values(♠) + 1.2 \times \sum [values(♦) + values(♥)]} $$

After computing the base score, calculate the penalty for use of ♣ (indicating weapons to protect your lair) and the bonus for use of ♦ (indicating high value gemstones):

$$ penalty = { \frac{\\# ♣}{\\# cards} }$$

$$ bonus = { \frac{\\# ♦}{\\# cards} }$$

Thus, score is now computed as follows:

$$ score_{tricks} =  (1 - penalty + bonus) \times base$$

You also lose score points for each card still in your hand.

$$ score = score_{tricks} - 2 \times \sum values (hand) $$

## Turns

**At the end of your turn, if you have less than 3 cards in your hand, you draw cards equal two the difference. Similarly, if you have more than 5 cards, discard the surplus cards.**

Each player's turn consists of up to 2 from the 3 available actions.
1. Hoard treasure.
2. Accumulate treasure.
3. Hoard stroll.

Each step can't be performed more than once. The order of the actions to be perforemed is left to the player themselves. (Some exeptions will be explained later).

### Dragon's Roar
> A dragon's roar echoes through the cosmos, a symphony of power unleashed. The very air quivers with the might of ancient forces. Thus, the dragon assert their dominance, turning the tide of fate with a thunderous declaration of their unparalleled strength and strategic prowess that reverberates across the realm.

As an extra action during their turn, the player can activate the special ability of a king (K) in their possesion. When the ability is <ins>resolved</ins>, the K card is returned to the <ins>hand</ins> of their original owner.

A K card in hand has a value of 0 and can't be played in any combination.

### Hoard treasure
> As sun slowly sets, dragons, triumphant in their quests, hoard treasures with majestic pride. The accumulated wealth, a testament to their might, is carefully played and stored, today's hunt proudly engraved in the annals of dragon lore.

***Play cards from your hand to store them in your vault.***

Cards can only be played as part of a combination. Available combinations are:
- a pair of cards of equal rank
- a trio of cards of equal rank
- all four cards of the same rank
- a sequence of length 3-5

Each player plays their cards face-down in front of them. 

Alternatively, a player can add to an already existent combination, if <ins>a single card</ins> matches (or the player bluffs it matches).

### Accumulate treasure
> In the dragon realms, wings unfurl in a quest for glory. The sun is high and dragons soar through uncharted skies, leaving behind a saga of epic conquest. The hunt for wealth echoes in thunderous roars, as mighty dragons pursue their destiny.

***Get more cards in your hand.***

There are many ways for a player to empower their collection of treasures.

#### 1. Draw 1/2/3 cards from the deck.
If more than one cards are drawn this way, <ins>only 1 is kept</ins> and the rest are discarded face-up.

#### 2. Get all cards from the discard pile.

#### 3. Raid a dragon's lair.
Either the active player randomly selects 1 card from an opponet's hand and adds it to their own hand, or the opponets selects 2 cards and gives them to the active player.

If the 2 players disagree on the action to be performed, with the active player calling, then a terrifying `dragon fight` will emerge!

- Both players reveal the card with the highest value among those in their hands.
- The player with the highest valued card gets to choose one of the two alternative actions.
- In case of a draw, the treasure hunt is unsuccessful. Both players discard the tied cards and draw new ones.

#### 4. Loot another dragon.
<ins>This option is available only if the active player has already used a `hoard treasure` action.</ins>

The active player selects any already played combination in any other player's hoard. The selected combination must have as many cards as the combination the current player used. The two players compare their loots (without showing to other players). The strongest dragon gets both!

<ins>The following rules are to be used in order of appearence.</ins>

- Since ♣ act as a defensive mechanism for a player's lair, the "defender" adds the value of any ♣ card(s) to the combination. 

    Example 1:

        {3@, 3♣} == {6@, 6@} , @:♥/♦/♠

    Example 2:

        {3@, 3@, 5♣} = {8@, 8@} , @:♥/♦/♠
        
    Example 3:

        {3♣, 4@, 5@, 6@, 7@} = {6@, 7@, 8@, 9@, 10@} , @:♥/♦/♠
    
    The maximum value of cards (J/Q=11) can't be surpassed.

    Example 4:

        {Q@, Q@} = {Q@, Q♣} , @:♥/♦/♠

    The comparison continues normally. At the end of the turn, before claiming loots, any ♣ not part of the combination (see example 2) are discarded.

- A combination containing non matching cards is invalid: The defender immediately loses. The active player claims the combination as theirs and the non-matching cards are discarded.
- In case of incompatible combinations both players simply discard a card.

    Example 5:
        
        {4%, 5%, 6%} ≟ {3%, 3%, 3%} , %:♥/♦/♠/♣

- The player with the greatest combination wins and gets both combinations in their hoard.
- In case of a draw each player returns the competing combination to their hand and have to discard a card.

### Hoard stroll
> The day was not suitable for a treasure hunt. It was a moment of strategic contemplation, a pause to navigate accumulated riches with poise. With a regal grace, did the monster embark on a hoard stroll, weaving through the treasures they've claimed. They felt happy, solidifying their status. Reassured.

***Gain information. Play special cards***

Using this action, the player can either see any number of the combinations they have already played <ins>or</ins> look at the top card of the library and put it back on top or bottom of the library.

Additionally, if the player has any king (K) cards in their hand, they may play those cards face up in their hoard.

## Clarifications / FAQ

### Order of cards

The order of cards is important for determining the winner during fights of the `accumulate treasure` actions.

    A < 2 < 3 < 4 < 5 < 6 < 7 < 8 < 9 < 10 < J = Q < A
