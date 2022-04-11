# discord_query_bot

# First of All
See Readme in [discord_bot]


# introduction
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

