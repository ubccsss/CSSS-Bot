# CSSS-Bot
A bot designed to track and promote user engagement on the UBC CSSS Official Discord server.

Built using [discord.py](https://pypi.org/project/discord.py/), with database connections to MongoDB. Deprecated SQLite DB connections can also be found in sqlite.py. You can see it in action in [our discord](https://discord.gg/bTQdVGSGCd) :)

## Usage
To run the bot, create a .env @ the root of this project with keys for `DISCORD_TOKEN`, as well as MongoDB keys regarding `DB_NAME`, `DB_CLUSTER`, and `DB_COLLECTION`. Then simply run in a pipenv.

## MongoDB Setup
This program is meant to interact with a database with two collections, 'members' and 'roles'. New react roles can be added by creating a document with the message id under 'id', as well as arrays for 'emojis' and 'roles' (must share the same index).

## License
This project is licensed under the [MIT License](https://github.com/cyruskalafchi/CSSS-Bot/blob/main/LICENSE). 
