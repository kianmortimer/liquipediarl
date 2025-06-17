# LiquipediaRL

**LiquipediaRL** is a Python wrapper for the [Liquipedia Rocket League site](https://liquipedia.net/rocketleague)

> This wrapper uses the official Liquipedia (MediaWiki) API and abides by the [TOS](https://liquipedia.net/api-terms-of-use)

---

## Examples

```python
from liquipediarl import LiquipediaRL

lp = LiquipediaRL(
    app_name="App Name",
    app_version="1.0.0",
    website="https://example.com",
    email="you@example.com"
)
```

## get_player()

```python
# Gets info for a specified player page
player = lp.get_player("SquishyMuffinz")

print(player.keys())
print(player['info']['earnings'])
print(player['settings']['camera'])
```
## get_all_players()

```python
# Gets all the Oceanic players
players = lp.get_all_player("Oceania")

print(len(players))
print(players[:5])

```

---



[@kianmortimer](https://github.com/kianmortimer)
