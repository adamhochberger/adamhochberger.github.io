## Overview
This page details progress and descriptions of different projects I have implemented (past and present). I have personal projects based in Python, Django, and Node.js, along with academic assignments and projects in React, MEAN stack, C++, and Java. 

---

## Current Projects

### [smite-wiki](https://github.com/adamhochberger/smitewiki) - Python/Django/React

A React single-page web application that asynchronously communicates with a Django REST API, which in turn uses a PostgreSQL SQL database to store and access application data according to the data model. The app utilizes information from the Smite Developer API and will serve up information in the form of a one-page app with the ability to easily compare items, gods, or relics (active items) in a more concise and detailed way than is currently available.
  
#### To be implemented

- Items app (model, views, URLs)
- Gods app (model, views, URLs)
- User app (model, views, URLs)
- Frontend pages

### [lol-wiki-bot](https://github.com/adamhochberger/lol-wiki-bot) - Node.js

A Discord.js (Node.js) based bot that retrieves information from this [League of Legends wiki site](https://leagueoflegends.fandom.com/wiki/League_of_Legends_Wiki) and sends it to the user in the same channel. This is intended for personal usage since I often discuss factors of the game with friends, but is still a publicly visible bot. This can also be used during the additional implementation of the [champion-calc project](https://github.com/adamhochberger/champion-calc) and may pull from that website in the future, rather than the wiki site. A roadmap of the progress on this project (Jira) is available [here](https://adamhochberger.atlassian.net/jira/software/projects/LWB/boards/1/roadmap).

#### Implemented

- `!champ [name] [ability_choice]`
  - Prints to user components of a champion's abilities (name, damage, cost)
  - `name` is a required field and verifies input with known list of all champions
  - `ability_choice` is one of  `q, w, e, r, or p(assive)` which denotes the ability for a champion - if left blank, it will print out passive and all abilities
- `!stats [name]`
  - Prints to user list of a champion's stats (health, mana, defense)
  - `name` is a required field and verifies input with known list of all champions
- `!item [name]`
  - Prints to user stats and passive of an item, along with gold efficiency and the recipe needed to create it
  - `name` is a required field and verifies input with known list of all items  
- `!tft [(t)rait] [name]`
  - Prints to user the stats and ability of a trait
  - `name` is a required field and verifies input with known list of all traits, champs, or items
  
#### To be implemented

- `!rune [name]`
  - Prints to user the information of a given rune (ability, skill tree)
- `!tft [(c)hamp, (i)tem] [name] -
  - Prints to user the stats and ability of a champion, or item from TFT
  - Functionality will be placed into the above implemented function of the same command

## Past Projects

### [Social Compass](https://github.com/adamhochberger/seatcheck-web) - React
A React-based team web application for senior project course, that also used Firebase for user and map storage. I created the front-end elements with the material-ui module in React, and made the home page, along with the user authentication pages. This website's goal was to help users find each other in different locations that they create through the web application or a connected mobile application. The website is hosted [here](https://socialcompass2020.herokuapp.com).

### [Study Spots](https://github.com/adamhochberger/study-spots) - MEAN Stack
A MEAN stack-based team web application created during my past Software Engineering course. The purpose of this website was to allow users to reserve rooms on campus and interact with users through voting on how good a room was. The website also utilizes the Mapbox API to display the markers for different buildings on the map. The data points were retrieved from an old University of Florida API and the corresponding images for the buildings were pulled from an index website from UF as well. This project also allows for user registration and login and was near completion, outside of bug testing, when submitted at the end of the semester. The website is hosted [here](https://study-spots-group3-1250-test.herokuapp.com).

### [Portfolio Website](https://github.com/adamhochberger/django-portfolio) - Python/Django
A repository that would serve as basis of personal portfolio website written in Django 3. The purpose of this website was to offer an interactive way for potential employers to view previous projects that have been created. Additionally, this can be utilized by myself as a form of dev-blog while working on personal projects. This code was not finished as I found other avenues to create a portfolio but will likely return to it in the future to function more as a development blog.
