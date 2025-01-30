# Teneo Node CLI

![teneo](image.png)

Teneo is a browser extension that allows you to earn $TENEO tokens by running a node that accesses public social media data. This CLI version provides an alternative way to run the Teneo node without using the browser extension.

## ⚠️ Disclaimer
I am not responsible for any account bans that may occur from using this CLI version. While I believe there is no reason for bans as this implementation follows the same rules as the official extension (15-minute heartbeats, 25 max points per cycle, 2400 max points per day), use this at your own discretion.

## Features
- ✅ Account registration
- ✅ Login with email/password
- ✅ Automatic token refresh
- ✅ WebSocket connection management
- ✅ Automatic reconnection
- ✅ Proxy support
- ✅ Multiple account support
- ✅ Cross-platform compatibility

## Installation

### Prerequisites
- Node.js (v16 or higher)
- npm (comes with Node.js)

### Termux (Android)
```bash
pkg update && pkg upgrade
pkg install nodejs git
git clone https://github.com/Fl3xxRichie/ten.git
cd ten
npm install
```

### Linux
```bash
sudo apt update
sudo apt install nodejs npm git
git clone https://github.com/Fl3xxRichie/ten.git
cd ten
npm install
```

### macOS
```bash
brew install node
git clone https://github.com/Fl3xxRichie/ten.git
cd ten
npm install
```

### Windows
1. Install Node.js from [nodejs.org](https://nodejs.org/)
2. Open Command Prompt or PowerShell:
```bash
git clone https://github.com/Fl3xxRichie/ten.git
cd ten
npm install
```

## Usage

### Single Account
```bash
npm start
```

### Multiple Accounts
1. Add accounts to `accounts.txt` (format: `email|password`)
2. Generate tokens:
```bash
node getToken.js
```
3. Start multiple nodes:
```bash
node multy.js
```

### Proxy Configuration (Optional)
Add proxies to `proxies.txt` (one per line) in the format:
```
http://username:password@host:port
```

## Project Structure
```
ten/
├── accounts.txt        # Store email|password credentials
├── proxies.txt         # Proxy configurations
├── tokens.txt          # Generated access tokens
├── localStorage.json   # Session storage
├── main.js             # Main application script
├── multy.js            # Multiple account handler
├── getToken.js         # Token generator
├── package.json        # Project dependencies
└── README.md           # This documentation
```


## Support
For issues and feature requests, please [open an issue](https://github.com/Fl3xxRichie/ten/issues) on GitHub.

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a pull request



## 🌐 Connect With Me

[![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?style=for-the-badge&logo=Twitter&logoColor=white)](https://twitter.com/FlexxRichie)
[![Telegram](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)](https://t.me/FlexxRichie)
[![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Fl3xxRichie)

## License

MIT License - See LICENSE file for details