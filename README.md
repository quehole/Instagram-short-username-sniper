# Instagram Username Checker

A simple Python-based Instagram username checker that generates random 5-character username combinations, checks them against Instagram's signup endpoint, and sends usernames classified as available to a Telegram bot.

> **Note:** This project uses an Instagram web endpoint and hardcoded request headers/cookies from an older implementation. It may no longer work reliably due to changes on Instagram.

## ✨ Features

* Generates random 3-5 character username combinations
* Uses letters, numbers, `_`, and `.`
* Checks generated usernames through Instagram's signup endpoint
* Displays results directly in the terminal
* Sends usernames classified as available to Telegram
* Includes colored terminal output and ASCII artwork

## 📋 Requirements

* Python 3.x
* `requests`

Install the dependency:

```bash
pip install requests
```

## 🚀 Usage

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd YOUR_REPOSITORY
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the script:

```bash
python main.py
```

The script will ask for:

```text
TELEGRAM USER ID ➤
TELEGRAM BOT TOKEN ➤
```

Enter your Telegram bot's credentials when prompted.

## 📁 Project Structure

```text
.
├── main.py
├── requirements.txt
└── README.md
```

### `requirements.txt`

```text
requests
```

## 🔧 How It Works

The script:

1. Generates random characters.
2. Builds several possible 5-character username combinations.
3. Selects one of the generated combinations.
4. Sends a request to Instagram's account creation endpoint.
5. Checks the response for indicators that the username is unavailable or the request was rate-limited.
6. Prints the result in the terminal.
7. When a username is classified as available, sends it to the configured Telegram bot.

## ⚠️ Disclaimer

This project is provided for **educational and research purposes**.

The script interacts with a third-party service and may be affected by changes to Instagram's APIs, anti-bot systems, rate limits, or terms of service.

You are responsible for how you use this software. Do not use it to spam, abuse, bypass platform protections, or violate the rules of services you interact with.

## 🔐 Security

**Do not commit Telegram bot tokens, cookies, CSRF tokens, or other credentials to GitHub.**

If you fork or modify this project, keep sensitive credentials out of source code and use environment variables or another secure configuration method.

## 👤 Author

**QUE**

`@queholes • @quehole`

---

⭐ If you found this project useful, consider starring the repository.
