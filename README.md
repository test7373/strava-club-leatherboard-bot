# Strava club - Week's Leaderboard

A Python project for scraping data from Strava club leaderboards using Selenium.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [License](#license)

## Introduction
* Based on https://github.com/sergbondckua/strava_club_last_week_leaderboard

* This Python code allows you to scrape data from Strava club leaderboards, providing information about club members, such as rank, distance. It uses [Selenium](https://www.selenium.dev/) to automate interactions with the [Strava](https://www.strava.com/) website.

* Scraped data send to users via telegram bot. [Inline](https://core.telegram.org/api/bots/inline) and classic 

* [![https://i.imgur.com/hPoMy52.png](https://i.imgur.com/hPoMy52.png)](https://i.imgur.com/hPoMy52.png)
## Installation
1. **Clone this repository:**

    ```bash
    git clone https://github.com/DmitryTeplov182/strava-club-leatherboard-bot.git
    ```
2. **Copy .env.template to .env and fill in the necessary data:**
   ```bash
   cp .env_dist .env
   ```
2. **Without Docker:**
   1.  Copy `.env_dist` to `.env` and fill in the necessary data.
   2. Create a [venv](https://docs.python.org/3/library/venv.html)
       ```bash
       cd strava-club-leatherboard-bot/
       ```
       ```bash
       python3 -m venv venv
       ```
       ```bash
       source venv/bin/activate
       ```
   3. Upgrade `pip`:
      ```bash
       pip install --upgrade pip
      ```
   4. Install dependencies from `requirements.txt`:
      ```bash
      pip install -r requirements.txt
      ```
   5. Run the project:
      Get stats:
      ```bash
      python main.py 
      ```
      Run bot
      ```bash
      python tg.py
      ```
3. **Docker:**
   1.  Copy `.env_dist` to `envs` dir and fill in the necessary data.
   2. Edit `docker-compose.yaml` and start it.
       ```bash
       docker compose up -d
       ```

## License
                    GNU GENERAL PUBLIC LICENSE
                       Version 3, 29 June 2007
