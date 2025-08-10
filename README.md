# 🔗 Ethereum Transaction Tracker

A sleek, real-time web application for monitoring Ethereum wallet transactions directly from the blockchain. Built with vanilla HTML, CSS, and JavaScript for maximum compatibility and performance.

![Ethereum Transaction Tracker](https://img.shields.io/badge/Ethereum-3C3C3D?style=for-the-badge&logo=Ethereum&logoColor=white)
![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

## ✨ Features

- **📱 Real-time Transaction Monitoring** - Watch Ethereum transactions as they happen
- **🔄 Auto-refresh Capability** - Automatically updates every 30 seconds
- **💎 Beautiful UI/UX** - Modern gradient design with smooth animations
- **📊 Comprehensive Transaction Details** - Hash, addresses, values, gas fees, timestamps, and block numbers
- **🎯 Address Validation** - Ensures only valid Ethereum addresses are tracked
- **📱 Fully Responsive** - Works perfectly on desktop, tablet, and mobile devices
- **🚀 Zero Dependencies** - Pure HTML/CSS/JavaScript - no frameworks needed
- **⚡ Fast Performance** - Lightweight and optimized for speed

## 🚀 Quick Start

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- An Etherscan API key (free from [etherscan.io](https://etherscan.io/apis))

### Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/ethereum-transaction-tracker.git
   cd ethereum-transaction-tracker
   ```

2. **Configure your API key**
   - Open `ethereum-tracker.html` in a text editor
   - Find line 234: `const apiKey = 'YOUR_API_KEY_HERE';`
   - Replace `YOUR_API_KEY_HERE` with your Etherscan API key

3. **Run the application**
   - Simply double-click `ethereum-tracker.html` to open in your browser
   - Or serve it from a local web server for best performance

## 🎯 Usage

1. **Enter a wallet address** - Paste any valid Ethereum address (starts with 0x)
2. **Click "Track Wallet"** - Start monitoring transactions in real-time
3. **View transaction details** - See comprehensive information for each transaction
4. **Toggle auto-refresh** - Enable/disable automatic updates
5. **Stop tracking** - Use the stop button to cease monitoring

### Example Wallet Addresses to Try
- Ethereum Foundation: `0xde0B295669a9FD93d5F28D9Ec85E40f4cb697BAe`
- Uniswap V3: `0x1F98431c8aD98523631AE4a59f267346ea31F984`
- OpenSea: `0x5b3256965e7C3cF26E11FCAf296DfC8807C01073`

## 🏗️ Technical Architecture

### Frontend Technologies
- **HTML5** - Semantic markup and structure
- **CSS3** - Modern styling with Flexbox/Grid and animations
- **Vanilla JavaScript** - ES6+ features for API integration and DOM manipulation

### API Integration
- **Etherscan API** - Official Ethereum blockchain data provider
- **RESTful calls** - Efficient data fetching with error handling
- **JSON parsing** - Clean data transformation and display

### Key Components
```
├── Transaction Display Engine
├── Real-time Data Fetcher  
├── Address Validator
├── Auto-refresh Manager
├── Responsive UI Controller
└── Error Handler
```

## 📊 Transaction Data Displayed

Each transaction card shows:
- **Transaction Hash** - Unique blockchain identifier
- **From/To Addresses** - Sender and recipient wallet addresses
- **Value** - Amount of ETH transferred
- **Gas Fee** - Transaction cost in ETH
- **Block Number** - Blockchain block containing the transaction
- **Timestamp** - When the transaction occurred
- **Status** - Success or pending state

## 🎨 UI/UX Features

- **Gradient backgrounds** with modern color schemes
- **Smooth animations** for new transactions and interactions
- **Hover effects** and micro-interactions
- **Status indicators** with color-coded feedback
- **Loading states** with elegant spinners
- **Error messages** with helpful troubleshooting tips
- **Mobile-first design** with responsive breakpoints

## 🔧 Configuration Options

### Auto-refresh Settings
- **Interval**: 30 seconds (configurable in code)
- **Toggle**: Can be enabled/disabled by user
- **Smart refresh**: Only when actively tracking

### Display Settings
- **Transaction limit**: 20 most recent transactions
- **Address format**: Shortened display (0x1234...5678)
- **Timestamp format**: Localized date/time

## 🛠️ Development

### Local Development Setup
```bash
# Clone and navigate
git clone https://github.com/yourusername/ethereum-transaction-tracker.git
cd ethereum-transaction-tracker

# For development with live reload (optional)
npx live-server --port=3000
```

### Code Structure
```
ethereum-tracker.html
├── <head>
│   ├── Meta tags and title
│   └── Embedded CSS styles
└── <body>
    ├── Header section
    ├── Input controls
    ├── Status bar
    ├── Transaction display
    └── Embedded JavaScript
```

### Key Functions
- `fetchTransactions(address)` - API calls to Etherscan
- `displayTransactions(transactions)` - Render transaction cards
- `startTracking()` - Initialize wallet monitoring
- `formatEther(wei)` - Convert Wei to ETH
- `updateStatus()` - Manage UI status indicators

## 🔒 Security & Privacy

- **Client-side only** - No data stored on external servers
- **API key protection** - Keys should be kept secure
- **Address validation** - Prevents invalid input
- **Error handling** - Graceful failure management
- **No tracking** - Zero user analytics or data collection

## 🚨 Troubleshooting

### Common Issues

**"Failed to fetch" errors:**
- Check your internet connection
- Verify your API key is valid
- Ensure the wallet address format is correct (42 characters, starts with 0x)

**CORS errors in some browsers:**
- Run from a local web server instead of file://
- Use browsers that support local file access
- Consider using a simple HTTP server

**No transactions showing:**
- Verify the wallet address has transaction history
- Check if the address is a contract vs. wallet address
- Try a different wallet address

### API Rate Limits
- Free Etherscan API: 5 calls/second, 100,000 calls/day
- Upgrade to Pro for higher limits if needed

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

### Development Guidelines
1. **Code Style** - Use consistent formatting and naming
2. **Comments** - Document complex functions and logic
3. **Testing** - Test with multiple wallet addresses
4. **Responsive** - Ensure mobile compatibility
5. **Performance** - Optimize for speed and efficiency

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Etherscan](https://etherscan.io/) for providing the excellent API
- [Ethereum Foundation](https://ethereum.org/) for the incredible blockchain technology
- The open-source community for inspiration and best practices

## 📞 Support

If you encounter any issues or have questions:
1. Check the troubleshooting section above
2. Open an issue on GitHub
3. Review the Etherscan API documentation

---

**Made with ❤️ for the Ethereum community**

*Star ⭐ this repository if you found it helpful!*
