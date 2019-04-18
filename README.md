# idle4x - Game Design Doc

4X idle game with massive multiplayer elements.

## Game Design

### The world
1. The player exists in a world shared with by all other players.
2. This world is reset every month.
3. Players may join at any time.
4. There is only one world.

### The player
1. Each player is the ruler of an intergalatic empire.
2. Each empire controls a certain amount of resources
  1. Food
  2. Materials
  3. Research Points
  4. Population
  5. Combat Power
  6. Territory
3. Each player is able to purchase upgrades/units/buildings/whatever
   that modify the amount of resources and/or the rate of production of
   resources

### Resources
1. Food
  1. Controls the population cap
  2. Increased by food generations (e.g. farms)
2. Materials
  1. Used to purchase most upgrades/units/buildings/whatever
  2. Produced by harvesters (e.g. mines)
3. Research Points
  1. Used to purchase scientific upgrades
  2. Produced by researchers (e.g. labs)
4. Population
  1. Used to run any buildings (e.g. mines, labs)
  2. Also used to "run" units
5. Combat power
  1. Increased by units
  2. Used for player to player combat
6. Territory
  1. Increased by winning battles in player vs player combat
  2. Used to determine the winning at the end of the month - essentially score.


### Combat
1. Each player is able to attack any other player
2. The propability of winning is based on each player's combat power.
3. Attacker has advantage.
4. When a player is attacked they are notified (push notification)
5. They are able to retaliate with a relatiation bonus (higher chance
   of victory and better rewards).
6. When a player is victorious they receive materials and research points 
   in proportion to the opponents
7. The attacking player will lose population and units upon victory or defeat.
8. The defending player if defeated will lose territory.
9. The attacking player if victorious will win territory.

## Technical Notes
1. Game is played in the browser, progressive web app.
2. Player can login to authenticate themselves.
3. Internet access is required.
4. Resource numbers can get very large (< 64 bit uint)
