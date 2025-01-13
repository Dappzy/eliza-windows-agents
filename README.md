# Eliza Windows Twitter Agents 🤖

A Windows-optimized fork of [Eliza](https://github.com/elizaos/eliza) with a focus on Twitter integration and character agents. After working with the original project, I noticed Windows users faced some unique challenges. This repository aims to provide clearer Windows-specific documentation and configurations, making it easier for Windows developers to get started.

## 🪟 Why This Fork?
- Original documentation assumed Unix-like environments
- Windows users faced path resolution issues
- Twitter integration needed additional Windows-specific configurations
- Some dependencies required Windows-specific workarounds

This fork maintains all the amazing features of Eliza while making life easier for Windows users!

## 📱 Connect & Support

<div align="center">
  
[![Telegram](https://img.shields.io/badge/Telegram-@DappChef-blue?style=for-the-badge&logo=telegram)](https://t.me/DappChef)
[![Twitter Follow](https://img.shields.io/badge/Twitter-Follow-blue?style=for-the-badge&logo=twitter)](https://twitter.com/intent/follow?screen_name=degendavegems)

Need help or interested in custom development work? 
- 💬 Reach out on Telegram: [@DappChef](https://t.me/DappChef)
- 🚀 Follow for updates on crypto integrations and cool features
- 🌟 If this helped you, a follow would be appreciated!

**Coming Soon:**
- 💎 Crypto-specific agent templates
- 🤖 Advanced trading bot integrations
- 🎮 GameFi automation tools

</div>

## 🚀 Windows-Specific Setup

### Prerequisites
- Node.js 18+ (LTS recommended)
- pnpm (Install using `npm install -g pnpm`)
- Git for Windows
- A Twitter/X account

### Installation Steps

1. **Clone and Install Dependencies**
```bash
git clone https://github.com/yourusername/eliza-windows-agents
cd eliza-windows-agents
pnpm install
```

2. **Environment Setup**
- Copy `.env.example` to `.env`
- Configure your Twitter credentials:
```env
TWITTER_USERNAME=your_username
TWITTER_PASSWORD=your_password
TWITTER_EMAIL=your_email
```

3. **Character Configuration**
- Characters are stored in `characters/*.character.json`
- Example configurations included for:
  - Dobby (crypto-helper character)
  - More characters coming soon...

### 🏃‍♂️ Running the Agent

```bash
# Start a specific character (e.g., Dobby)
pnpm run start -- --character characters/dobby.character.json
```

## 🔧 Windows-Specific Changes

1. **Path Handling**
- Fixed path resolution issues on Windows
- Updated file separators for Windows compatibility

2. **Twitter Integration**
- Added proper Windows environment variable handling
- Configured Twitter client for Windows environments
- Added email field for Twitter authentication

3. **Model Configuration**
- Set up OpenRouter integration with Mistral model
- Configured for optimal performance on Windows

## 📝 Usage

1. **Twitter Agent Setup**
- Configure target accounts in `.env`:
```env
TWITTER_TARGET_USERS=user1,user2
```
- Agent will monitor and interact with specified accounts
- Customizable interaction frequency and behavior

2. **Character Customization**
- Edit character files in `characters/` directory
- Customize personality, responses, and behavior
- Add new characters as needed

## 🤝 Contributing

Feel free to:
- Add new character configurations
- Improve Windows compatibility
- Fix bugs
- Add new features

## ⚠️ Known Issues & Solutions

1. **React Hook Errors**
- If encountering "Invalid hook call" error, run the agent directly instead of using web interface

2. **Path Issues**
- Use forward slashes (/) in configuration files
- Or escape backslashes (\\) properly

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---
*This is a modified version of Eliza, optimized for Windows and Twitter integration. For the original project, visit [Eliza's GitHub repository](https://github.com/elizaos/eliza).*
