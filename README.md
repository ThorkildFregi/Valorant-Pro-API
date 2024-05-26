# Valorant-Pro-API

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Presentation**

A python library to retrieve data from pro matches of valorant registered on the site https://vlr.gg/.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Installation**

*Step 1 :*

Create a new environment with conda or venv.

*Step 2 :*

Clone the repositery in your project's file.

```bash
git clone https://github.com/ThorkildFregi/wikidata-image-classifier/
```

*Step 3 :*

Install the dependencies :

```bash
pip install beautifulsoup4
```

OR

*Step 1 :*

Create a new environment with conda or venv.

*Step 2 :*

Install the dependencies :

```bash
pip install beautifulsoup4
```

*Step 3 :*

Install it with pip :

```bash
pip install ValorantProAPI
```

-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

**Utilisation**

*data.get_events()* (Function)

Use it to retrieve all the event's id and name from https://vlr.gg/

*data.Event* (Class)

This is the class of an event. To call it, you need the event id.

Example to retrieve data from Champions Tour 2024: EMEA Stage 1 :
```python
data.Event("1998")
```

*data.Event.name*

To get the event name.

