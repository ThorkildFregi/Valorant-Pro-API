# Valorant-Pro-API

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Presentation**

A python library to retrieve data from pro matches of valorant registered on the site https://vlr.gg/.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Installation**

*Step 1 :*

Create a new environment with conda or venv.

*Step 2 :*

Install the dependencies :

```bash
pip install beautifulsoup4, requests
```

*Step 3 :*

Install it with pip :

```bash
pip install Valorant-Pro-API
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Utilisation**

--------------------------------

*data.get_events()* (Function)

Use it to retrieve all the event's id and name from https://vlr.gg/

----------------

*data.Event* (Class)

This is the class of an event. To call it, you need the event id.

Example to retrieve data from Champions Tour 2024: EMEA Stage 1 :
```python
data.Event("1998")
```

----------------

*data.Event.id*

To get the event id.

----------------

*data.Event.name*

To get the event name.

----------------

*data.Event.matches*

To get the match's id of the event.

--------------------------------

*data.Match*

This is the class of a match. To call it, you need the match id.

Example to retrieve data from BBL Esports VS Gentle Mates :
```python
data.Match("318917")
```

----------------

*data.Match.id*

To get the match id.

----------------

*data.Match.winner*

To get the match winner.

----------------

*data.Match.rounds*

To get the round's id of the match.

----------------

*data.Match.team_a.name*

To get the name of team A.

----------------

*data.Match.team_a.score*

To get the score of team A.

----------------

*data.Match.team_b.name*

To get the name of team B.

----------------

*data.Match.team_b.score*

To get the score of team B.

--------------------------------

*data.Round*

This is the class of a round. To call it, you need the round id and the match id.

Example to retrieve data from BBL Esports VS Gentle Mates Round 1 :
```python
data.Round("164106", "318917")
```

----------------

*data.Round.id*

To get the round id.

----------------

*data.Round.match_id*

To get the match id.

----------------

*data.Round.map*

To get the map of the round.

----------------

*data.Round.winner*

To get the winner of the round.

----------------

*data.Round.team_a.name*

To get the name of team A.

----------------

*data.Round.team_a.score*

To get the score of team A.

----------------

*data.Round.team_a.player_{1 to 5}*

This is the player of the team under a form of class.

----------------

*data.Round.team_b.name*

To get the name of team B.

----------------

*data.Round.team_b.score*

To get the score of team B.

----------------

*data.Round.team_b.player_{1 to 5}*

This is the player of the team under a form of class.


--------------------------------

*data.Player*

This is the class of a player. You don't need to call it, it's in *data.Round.team_{a or b}.player_{1 to 5}*.

----------------

*data.Player.name*

To get player name.

----------------

*data.Player.country*

To get player country.

----------------

*data.Player.agent*

To get player agent.

----------------

*data.Player.stat*

To get the stats.

--------------------------------
