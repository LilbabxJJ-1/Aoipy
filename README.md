# AoiPy - Discord.py made simple
Latest Update: 12/13/22

![PyPI](https://img.shields.io/pypi/v/aoipy)
![PyPI - Downloads](https://img.shields.io/pypi/dm/aoipy?color=green&label=downloads)
![Downloads](https://static.pepy.tech/personalized-badge/aoipy?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)
![PyPI - License](https://img.shields.io/pypi/l/aoipy)
![](https://tokei.rs/b1/github/tomschimansky/aoipy)

![AoiPY](https://github.com/LilbabxJJ-1/Aoipy/blob/master/aoipy/AOIpy%20(1).png)
### Using AoiPy
1 - `pip install AoiPy`

2 - Import Client and any other files

```python

from aoipy.Client import client
from aoipy.File import * 
```

3 -  Example:

```python

from aoipy.Client import *
from aoipy.Messages import *
import discord
# ---------------Imports--------------------
act = client.activity("tv", "watching")
bot = client.Bot(prefix="!", case_insensitive=False, intents=("all",), activity=act)
events = client.Events()

@events.onReady
def startup():
    print(f"{botUsername()} is ready!")


@bot.command()
async def ping(ctx):
    await sendChannelMessage(ctx, "Pong!")


bot.run("*******<<TOKEN>>***********")
```

Bare Minimum bot
```python
from aoipy.Client import *
bot = client.Bot(prefix="!", intents=("all",))
events = client.Events()

@events.onReady
def startup():
    print(f"{botUsername()} is ready!")
```
## New and still a work in progress
