# Adam Hochberger's portfolio

This website features progress of different source repositories and past projects

---

## Current Projects

### [lol-wiki-bot](https://github.com/adamhochberger/lol-wiki-bot)

A Discord.js (Node.js) based bot that retrieves information from this [League of Legends wiki site](https://leagueoflegends.fandom.com/wiki/League_of_Legends_Wiki) and sends it to the user in the same channel. This is intended for personal usage since I often discuss factors of the game with friends, but is still a publicly visible bot. This can also be used during the additional implementation of the [champion-calc project](https://github.com/adamhochberger/champion-calc) and may pull from that website in the future, rather than the wiki site.

#### Functionality

##### Implemented

- `!champ [name] [ability_choice]`
  Prints to user components of a champion's abilities (name, damage, cost)
  - `name` is a required field and verifies input with known list of all champions
  - `ability_choice` is one of  `q, w, e, r, or p(assive)` which denotes the ability for a champion - if left blank, it will print out passive and all abilities
- `!stats [name]`
    Prints to user list of a champion's stats (health, mana, defense)
  - `name` is a required field and verifies input with known list of all champions

##### To be implemented

- `!item [name]` (*in progress*)
    Prints to user list of a item's stats (health, mana, defense) and passive

### [champion-calc](https://github.com/adamhochberger/calc)

A Python-based application that retrieves information from the League of Legends Data Dragon and Community Dragon APIs and uses it to perform calculations on champion objects. Currently, this project uses the `requests` package to query the API and save information into a local champion object class. Once the information is able to obtained and saved properly, I plan to change this into a web application. This project will use Django in the future to serve as a web application and will utilize PostgreSQL as the backend for storing champion objects that are created.

#### Functionality

##### Implemented

- Perform queries on the Data Dragon and Community Dragon APIs
- Pull champion stat into object and display
- Calculate champion stat adjustment based on level

##### To be implemented

- Create item class
  - Include attributes, passive
  - Perform data verification
- Convert champion/item object structure into PostgreSQL database designs
- Create Django project to perform queries and display data
- View champion information from individual URLs
- Implement calculator page where characters are manipulated
  - Add level scaling toggle
  - Add item to character and reflect changes
  - Show current damage of ability
- Extend base unit class for additional characters (minions, monsters)

## Past Projects (WIP)

