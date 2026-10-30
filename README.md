🤖 C++ Telegram Bot

A Telegram bot project written in C++. This project is intended for learning C++, API integration, and bot development.

✨ Features

- Built with C++
- Integrates with the Telegram Bot API
- Reads the bot token from an environment variable
- Designed for learning and further development

🛠️ Requirements

- Linux (tested on Arch Linux)
- A C++ compiler ("g++")
- Git
- A Telegram bot token from "@BotFather" (https://t.me/BotFather)
- "libcurl" if your code uses it for HTTP requests

📦 Installation

Install the required tools on Arch Linux:

sudo pacman -S --needed base-devel git curl

If your bot uses "libcurl", install it too:

sudo pacman -S --needed curl

Clone the repository:

git clone https://github.com/mokarimicom/cpp-telegram-bot.git
cd cpp-telegram-bot

🔑 Configuration

Set your Telegram bot token as an environment variable:

export TELEGRAM_BOT_TOKEN="YOUR_BOT_TOKEN"

Replace "YOUR_BOT_TOKEN" with your real token. Do not commit your token to GitHub.

🚀 Compile and Run

If your source file is named "main.cpp" and uses "libcurl":

g++ -std=c++17 -Wall -Wextra main.cpp -o bot $(pkg-config --cflags --libs libcurl)
./bot

If your project uses another HTTP library or build system, adjust these commands accordingly.

🔒 Security

- Never publish your Telegram bot token.
- Keep credentials out of source code and Git history.
- Use ".gitignore" to exclude ".env" files and compiled binaries.
- If a token is exposed, revoke it through "@BotFather" (https://t.me/BotFather).

📁 Project Structure

cpp-telegram-bot/
├── main.cpp
├── README.md
└── .gitignore

🎯 Learning Goals

- Practice modern C++
- Learn HTTP API integration
- Understand environment variables
- Learn Git and GitHub workflows

📜 License

Choose and add a license before distributing this project.

---

Created as a learning project for C++ and Telegram bot development.