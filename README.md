# Crypto Position Size Calculator

A free, open-source position size calculator designed for cryptocurrency traders. Calculate your trade size based on risk percentage or capped investment amount, with support for all crypto pairs.

## Features

- ✅ **Supports All Crypto Pairs** - Works with BTC, ETH, SOL, XRP, and any other cryptocurrency
- 📊 **Two Calculation Modes**:
  - **Risk Percentage Mode**: Calculate position size based on % of capital you want to risk
  - **Capped Investment Mode**: Set a maximum investment amount per trade
- 💰 **Real-time Price Integration** - Optional Bybit API integration for automatic price fetching
- 📈 **Take Profit Targets** - Automatic TP2 and TP3 calculations (2x and 3x profit targets)
- 📋 **Copy to Clipboard** - Quick copy functionality for coins to buy and TP values
- 💾 **LocalStorage** - Remembers your settings (capital, risk %, max investment)
- 🎨 **Modern UI** - Clean, responsive design with glass morphism effects
- 🔒 **Privacy First** - All calculations happen in your browser, no data sent to servers

## How to Use

### Option 1: Select a Bybit Pair (Auto Price)
1. Search and select your crypto pair from the dropdown (e.g., BTCUSDT)
2. Click the refresh button to fetch the current price
3. Enter your stop loss and optional take profit
4. View your calculated position size

### Option 2: Manual Entry (Any Pair)
1. Skip the pair selection or leave it empty
2. Manually enter the current price of your crypto
3. Enter your stop loss and optional take profit
4. View your calculated position size

### Calculation Modes

**Risk % Mode:**
- Set the percentage of your total capital you want to risk
- Calculator determines how many coins to buy based on your stop loss

**Capped $ Mode:**
- Set a maximum dollar amount to invest per trade
- Calculator shows your actual risk percentage

## Installation & Deployment

### Local Usage
Simply open the `crypto-position-calculator.html` file in any modern web browser.

### Deploy Online (Free Options)

#### 1. GitHub Pages
```bash
# Create a new repository
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/crypto-calculator.git
git push -u origin main

# Enable GitHub Pages in repository settings
# Your site will be live at: https://yourusername.github.io/crypto-calculator/
```

#### 2. Netlify
- Drag and drop the HTML file to [Netlify Drop](https://app.netlify.com/drop)
- Or connect your GitHub repository for automatic deployments

#### 3. Vercel
```bash
npm i -g vercel
vercel
```

#### 4. Cloudflare Pages
- Connect your GitHub repository at [Cloudflare Pages](https://pages.cloudflare.com/)
- Automatic deployments on every push

## Technologies Used

- **HTML5** - Semantic markup
- **Tailwind CSS** - Utility-first styling (via CDN)
- **Alpine.js** - Lightweight reactive framework (via CDN)
- **Bybit Public API** - Optional price data (no API key required)

## File Structure

```
crypto position size/
├── crypto-position-calculator.html   # Single-page application (all-in-one)
└── README.md                         # Documentation
```

## API Integration

The calculator uses Bybit's public API for fetching crypto pair prices:

**Endpoint:** `https://api.bybit.com/v5/market/tickers?category=spot`

No API key required. The API is used optionally - you can always enter prices manually.

## Browser Compatibility

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Opera (latest)

## Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Disclaimer

This tool is for educational and informational purposes only. It does not constitute financial advice. Always do your own research and consult with a financial advisor before making investment decisions. Cryptocurrency trading carries risk of loss.

## Support

If you find this tool helpful, consider:
- ⭐ Starring the repository
- 🐛 Reporting bugs or issues
- 💡 Suggesting new features
- 📢 Sharing with other traders

## Roadmap

Potential future features:
- [ ] Multiple currency support (EUR, GBP, etc.)
- [ ] Dark/Light mode toggle
- [ ] Export trade plan as PDF
- [ ] Support for additional exchange APIs
- [ ] Leverage calculator
- [ ] Risk/Reward ratio visualization
- [ ] Trade journal integration

## Contact

For questions, suggestions, or issues, please open an issue on GitHub.

---

**Made with ❤️ for the crypto trading community**
