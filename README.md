# Telegram Group Moderation Bot (aiogram)

This is a Telegram bot built using **Aiogram 3** (asynchronous Python Telegram framework) designed to help moderate group chats. The bot detects and removes messages containing offensive language or promotional/spam content, and applies temporary restrictions to rule violators.

## Features

* ✅ Welcomes users with `/start`
* ✅ Sends group rules with `/rules`
* ✅ Offers help using `/help`
* ✅ Automatically deletes join/leave notifications
* ✅ Detects and removes messages containing:

  * Profanity (loaded from a JSON file)
  * Advertisement links (URLs, Telegram links, common keywords)
  * Mentions (e.g. `@shavkatjon_mirzavaliyev`)
* ✅ Temporarily restricts users who send offensive content
* ✅ Skips admin messages from checks

---

## Installation

1. **Clone the repository:**

```bash
git clone https://github.com/Mirzavaliyev/qoravulbot.git
cd group-moderation-bot
```

2. **Create and activate a virtual environment :**

```bash
python -m venv .venv
source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`
```

3. **Install dependencies:**

```bash
pip install -r requirements.txt
```

4. **Prepare your JSON file for offensive words:**
   Create a file named `haqoratli_sozlar.json` in the same directory with the following structure:

```json
{
  "hate_words": ["badword1", "badword2", "..."]
}
```

5. **Edit your bot token:**
   Replace the `API_TOKEN` value in the script with your actual Telegram bot token.

---

## Running the Bot

```bash
python bot.py
```

The bot will begin polling and handle messages in real-time.

---

## File Structure

```
qoravulbot/
├── bot.py                 # Main bot logic
├── haqoratli_sozlar.json # JSON file with offensive words
├── requirements.txt       # Dependencies
└── README.md              # Documentation
```

---

## Requirements

* Python 3.8+
* Aiogram 3+

Install dependencies using:

```bash
pip install aiogram
```

---

## Deployment Ideas

You can run this bot on a VPS (like DigitalOcean), a local server, or deploy it on services like:

* Heroku
* Railway
* PythonAnywhere
* Docker container

---

## License

This project is open source and available under the MIT License.

---

## Author

Made by Shavkatjon Mirzavaliyev ✨
If you use this bot or find it useful, give the repository a star and feel free to contribute!

---

## TODOs

* [ ] Add logging
* [ ] Admin control panel
* [ ] Dynamic rule updates
* [ ] Multilingual support
