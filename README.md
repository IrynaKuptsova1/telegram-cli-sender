# Telegram CLI Sender

Challenge: Console command -> Telegram message or photo

Example:
```bash
$ bun run bot.ts message "Hello from the terminal"
Message sent!

$ bun run bot.ts photo "./images/photo.jpg"
Photo sent!
```

How to Run:
```bash
# Install dependencies
npm install

# Create a .env file with your Telegram credentials
BOT_TOKEN=your_telegram_bot_token
CHAT_ID=your_telegram_chat_id

# Run with Bun
bun run bot.ts message "Hello from the terminal"
bun run bot.ts photo "./path/to/photo.jpg"

# Short aliases
bun run bot.ts m "Hello from the terminal"
bun run bot.ts p "./path/to/photo.jpg"
```

This project turns simple terminal commands into Telegram messages and photo uploads, so you can send updates without opening a chat window. It uses TypeScript, Commander.js for the CLI, dotenv for environment variables, and the native Telegram Bot API through `node-telegram-bot-api`.
