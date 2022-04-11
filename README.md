# discord_query_bot

Bot to return query keyword and update pics and download button

The purpose of this project is like following:

- discord_bot.py is the bot script. 

- It adds a slash command /colour to invoke [MovieInfo](https://github.com/crvideo/MovieInfo) to seach a keyword in two avideo websites. 

[/colour keyword](./img/1.png)

- The results will generate several lines of drop select options. 

[options](./img/2.png)

- After you choose an option, the pics for the video will embed in the discord message.

[embed](./img/3.png)

- A download button will appear below the select options.

- By pressing the download button, the bot will query the specific video using [raincoat_prowlarr](https://github.com/crvideo/raincoat). The json results including download link will be returned in background.

- The download link will be sent to approprate downloading client to download it.

[downloading](./img/4.png)

# requisites

## python packages for build

- disnake
- disnake.ext
- subprocess
- json
- pprint
- re
- pathlib
- argparse
- urllib.parse
- shutil
- os.path


## other packages

- MovieInfo: included in this repo

- raincoat-prowlarr: included in this repo

- discord_bot: included in this repo

- loaded indexers in Jackett/Prowlarr




# usage

```{bash, label = "", linewidth = 85, eval=opt$eval}

python discord_bot/discord_bot.py 

```


# Config file
Put the config file in $HOME/.config/discord_query_bot.json


{
    "test_guilds": a long number,
    "token": "a long str"
}


- test_guilds (int)
  - This is the server name. You can right click onthe server and copy id to find it. Specifying test_guilds to accelerate deployment of your bots, which facilitate of debuging.

- token (str)
  - This is the token of your bot. You create a bot, give it the right permissions and generate a token.
  
  


# Acknowledgement

I am totally newhand to develop this project. It's workable but not fancy.
