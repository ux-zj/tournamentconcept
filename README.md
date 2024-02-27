# Triathlon style tournament organisation

Objectives of this tool in MVP:
- Allow users to quickly sign up to tournaments from any device.
- Allow tournament creators to add multiple stages to their tournaments, each stage can have its own activity.

## Concept Design
![alt text](docs/4.png)

## System Design
### Backend Tournament Service
![alt text](docs/1.png)

#### Tournament Formats
All tournaments begin with a cumulative leaderboard, where all participants have their points set to 0.

**Free for All**
- Participants are inserted into random seeds in the internal leaderboard for its stage.
  
**Gauntlet**
- This is a mono-branch single-elimination bracket.
- First game is played by the lowest seeded players, winner advances to play the next seed.
- Continue down this line until the winner reaches first seed for the final.
  
**Round Robin**
- A round-robin tournament (or all-play-all tournament) is a competition in which each contestant meets every other participant, usually in turn.

### Database (ERD)
![alt text](docs/2.png)

### MVP concept
![alt text](docs/3.png)
