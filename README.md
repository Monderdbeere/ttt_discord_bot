# TTT Discord Bot ![Icon](https://raw.githubusercontent.com/marceltransier/ttt_discord_bot/master/images/icon/icon_64x.png)

>Dead players can't speak!

*... and that's basically what this bot does.*

[![price](https://img.shields.io/badge/price-free-brightgreen.svg)](LICENSE)
[![gmod-addon](https://img.shields.io/badge/gmod-addon-_.svg?colorB=1194EF)](https://wiki.garrysmod.com)
[![discord-bot](https://img.shields.io/badge/discord-bot-_.svg?colorB=8C9EFF)](https://discord.js.org)
![i-like-badges](https://img.shields.io/badge/worlds--coolest--color-green-_.svg?colorB=00FF00)
[![license](https://img.shields.io/github/license/marceltransier/ttt_discord_bot.svg)](LICENSE)


This is a powerful [discord bot](https://discord.js.org) that mutes dead players in [TTT](http://ttt.badking.net) (Garry's Mod - Trouble in Terrorist Town)

## Getting Started
If you don't know how to install MySQL or Nodejs on your server, follow my [step-by-step guide on steam]()
### Prerequisites
- You have to have allready installed a Garry's Mod Server with the TTT Gamemode
- You must have MySQL and [Nodejs](https://nodejs.org) installed
- You need [Mysqloo](https://github.com/FredyH/MySQLOO) installed on you Garry's Mod Server (follow the [install instructions](https://github.com/FredyH/MySQLOO/blob/master/README.md#install-instructions))

### Installation
1. Clone this repository into your addons folder and install the requirements
     ```bash
     git clone https://github.com/marceltransier/ttt_discord_bot.git
     npm install --prefix ./ttt_discord_bot/discord_bot/
     ```
2. Rename config.json.example in config.json

3. Create Discord Bot, invite him to your server and paste the token in the config

   - if you don't know how to, follow [this guide](https://github.com/reactiflux/discord-irc/wiki/Creating-a-discord-bot-&-getting-a-token)
   
   - insert the bot token at `discord -> token` in the config.json
   
4. Insert the Guild *(Server)* id and the channel id in the config

   - if you don't know how to get these id's, follow [this guide](https://support.discordapp.com/hc/en-us/articles/206346498-Where-can-I-find-my-User-Server-Message-ID-)
   
   - insert the guild id at `discord -> guild` and the cannel id of the voice channel in wich the bot should mute dead players at `discord -> channel` in the config.json
      
5. Setting up MySQL

   - Create a MySQL database and user with privileges on the database for the bot
   - insert the MySQL host, user, password and database in the config.json


### Usage

- Start the bot by runing the node command with the `ttt_discord_bot/discord_bot/` directory
- Connect your Steam Account with the bot by typing `!discord YourDiscordTag` in the ingame chat. E.g `!discord marcel.js#4402`
- If you're **dead in Garry's Mod**, the **game-state is in progress**, you're **connected with discord** and you're in the **configured voice channel**, the bot will mute you. 

## Credits

- I used [discord.js](https://discord.js.org) in this project. Thanks for the easy opportunity writing a discord bot in javascript!
- Thanks for the great Garry's Mod gamemode [Trouble in Terrorist Town](http://ttt.badking.net) I made this bot for.

## Contributing

1. Fork it (<https://github.com/marceltransier/ttt_discord_bot/fork>)
2. Create your feature branch (`git checkout -b feature/fooBar`)
3. Commit your changes (`git commit -am 'Add some fooBar'`)
4. Push to the branch (`git push origin feature/fooBar`)
5. Create a new Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
