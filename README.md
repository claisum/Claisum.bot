# Claisum.bot - Discord Bot

A Discord bot built with discord.py

## 📋 Setup

### 1. Create a Discord Bot

- Go to [Discord Developer Portal](https://discord.com/developers/applications)
- Click "New Application" and name it
- Go to "Bot" section and click "Add Bot"
- Copy the token under the USERNAME section
- Paste it in `.env` file as `DISCORD_TOKEN`

### 2. Install Dependencies

```bash
# Create a virtual environment (recommended)
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On macOS/Linux:
source venv/bin/activate

# Install requirements
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Copy `.env.example` to `.env` and add your bot token:

```bash
cp .env.example .env
```

Edit `.env` and replace `your_bot_token_here` with your actual bot token.

### 4. Run the Bot

```bash
python bot.py
```

You should see:
```
YourBotName has connected to Discord!
------
```

## 🎮 Commands

- `!hello` - Bot greets you
- `!ping` - Check bot latency
- `!echo <message>` - Echo a message back

## 🔐 Add Bot to Your Server

1. Go to "OAuth2" > "URL Generator" in Developer Portal
2. Select scopes:
   - `bot`
3. Select permissions:
   - `Send Messages`
   - `Read Messages/View Channels`
4. Copy the generated URL and open it in your browser
5. Select your server and authorize

## 📚 Next Steps

- Add more commands in `bot.py`
- Create cogs for better organization
- Add event handlers
- Implement database integration
- Deploy to a hosting service (Heroku, Railway, etc.)

## 📖 Resources

- [discord.py Documentation](https://discordpy.readthedocs.io/)
- [Discord.js Guide](https://discordjs.guide/)
- [Discord Developer Portal](https://discord.com/developers/applications)

## ⚠️ Important

Never commit your `.env` file with your token! It's already in `.gitignore`.

---

Made with ❤️
