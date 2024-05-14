# Map Desiderata

## Problems With Vanilla H4

- Managing many towns and armies is annoying
- Optimal play involves micromanaging creature dwellings on the adventure map
  (via caravans / camping)
- Magic resistance is OP

## Goals

- Exploration
- Sense of place
- Surprise
- Leveling / progression
- Variety of creatures / hero types (maybe achieved through multiple plays?)
- Multiplayer- and AI-compatible
- Non-conquest victory
- Clear sense of who is ahead

## Anti-Goals

- Micromanaging small armies to do things like buy creatures and items
- TPKs / getting knocked out of a multiplayer game
- Traveling for many turns to get to the next destination
- Managing more than 3 towns
- Superhero barbarians
- Permanent hero imprisonment

## Possible Patterns

- Start on grass
- Chapters / Boundaries
- No creature dwellings outside towns
- No Caravans
- Armies without heroes can't move through certain border gates
- Random monsters attack armies without heroes
- Heroes who know Town Gate
- ~~Reduced creature growth in towns to make the game more hero-focused~~
  - Not technically possible AFAICT
- Portals home
- Scoreboard
- Emperor's Treasure
- Oracles
- Ring of Greater Negation
- Asymmetrical objectives? (good guys have shielded towns and must win by conquest; bad guys trying to collect artifacts)
- Creature dwellings continuously revert to "no owner"
  - makes it infeasible to camp dwellings with small armies
- Win by capturing 4 towns
- Progressive dungeons unlocked by keymaster tents

## Scripts

Run `Dwellings.ClearOwner` continuously or daily to prevent dwelling camping.
Note that multiple creature dwellings can define handlers for this event.

```
# Dwellings.ClearOwner
CHANGE OWNER to "No Player"
```
