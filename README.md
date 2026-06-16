# ZUSDD Mini App 💎

A Telegram Mini App for the ZUSDD cryptocurrency token - built for the Afghan community.

## 🌟 Features

### User Management
- **User Profile** - Display user information and avatar from Telegram
- **Balance Tracking** - Real-time balance display in ZUSDD tokens

### Trading
- **Buy Tokens** - Purchase ZUSDD tokens with custom amounts
- **Sell Tokens** - Sell your ZUSDD tokens with balance validation
- **Transfer Tokens** - Send tokens to other wallet addresses

### Market Data
- **Live Price** - Current token price with real-time updates
- **24h Change** - Price percentage change with visual indicators (📈 📉)
- **Market Statistics**:
  - Market Cap
  - 24h Trading Volume
  - Total Token Holders

### Referral System 🏆
- **Referral Codes** - Generate unique referral codes for each user
- **Commission Tracking** - 5% commission on referral transactions
- **Referral Count** - Track number of successful referrals

### User Experience
- **Toast Notifications** - Feedback messages for all actions
- **Haptic Feedback** - Vibration feedback on Telegram (light impact)
- **Responsive Design** - Mobile-optimized interface
- **Glassmorphism UI** - Modern design with blur effects

## 🛠️ Technology Stack

- **HTML5** - Structure and semantic markup
- **CSS3** - Modern styling with gradients and backdrop filters
- **JavaScript (Vanilla)** - No dependencies, pure JS
- **Telegram Web App API** - Integration with Telegram Mini Apps

## 📱 Telegram Integration

This app uses the official Telegram Web App API:
- `telegram-web-app.js` - Provides WebApp context
- `tg.initDataUnsafe.user` - Access user information
- `tg.HapticFeedback` - Trigger haptic feedback
- `tg.MainButton` - Control main action button

## 🚀 Getting Started

### Prerequisites
- Telegram Bot with Mini App enabled
- Web server to host the HTML file (HTTPS required)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/zait-noori/zusdd-mini-app.git
cd zusdd-mini-app
```

2. Host the `index.html` file on a web server

3. Configure your Telegram Bot's Mini App URL to point to your hosted file

4. Open the Mini App from your Telegram bot

### Quick Deploy

For quick testing, you can use any web hosting service:
- Netlify
- Vercel
- GitHub Pages
- Firebase Hosting

## 📊 Features Breakdown

### Price Updates
- Automatic price updates every 10 seconds
- Random price fluctuation (±0.1%) to simulate real market
- Price history tracking (last 7 prices)

### Balance Management
- Client-side balance tracking (can be extended to backend)
- Transaction validation before sell/transfer
- Insufficient balance error handling

### Referral System
- Unique code: `ZUSDD` + User ID
- Copy-to-clipboard functionality
- Commission rate: 5% per referral

## 🎨 Design Features

- **Color Scheme**:
  - Primary Gold: #ffd700
  - Dark Background: Gradient (#0f0c29, #302b63, #24243e)
  - Success Green: #00ff88
  - Error Red: #ff4444

- **Typography**: 
  - Supports Pashto language (افغانی)
  - Responsive font sizes
  - Clear visual hierarchy

- **UI Elements**:
  - Glassmorphism cards with backdrop blur
  - Smooth transitions and hover effects
  - Mobile-first responsive design

## ⚙️ Configuration

You can customize the following in the JavaScript section:

```javascript
// User defaults
let user = { first_name: "کارن", id: Math.floor(Math.random() * 1000000) };

// Initial price
let price = 0.024;

// Price history
let priceHistory = [0.0235, 0.024, 0.0245, 0.0238, 0.0242, 0.024];

// Referral commission
const REFERRAL_COMMISSION = 5; // 5%

// Price update interval
const UPDATE_INTERVAL = 10000; // 10 seconds
```

## 📈 Future Enhancements

- [ ] Backend integration for persistent data
- [ ] Real API integration for live market data
- [ ] Transaction history and analytics
- [ ] Wallet analytics dashboard
- [ ] Multi-language support
- [ ] Dark/Light theme toggle
- [ ] Push notifications
- [ ] KYC/AML verification
- [ ] Payment gateway integration
- [ ] Advanced charting
- [ ] Mobile app versions

## 🔒 Security Considerations

This is a client-side demo. For production deployment:
- ✅ Implement server-side validation
- ✅ Use secure API endpoints (HTTPS)
- ✅ Add authentication & authorization
- ✅ Implement rate limiting
- ✅ Store sensitive data securely
- ✅ Add CSRF protection
- ✅ Sanitize user inputs
- ✅ Never hardcode secrets
- ✅ Use environment variables for config
- ✅ Regular security audits

## 📱 Browser Support

- Chrome (Latest)
- Firefox (Latest)
- Safari (Latest)
- Telegram In-App Browser (Recommended)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📞 Support

For issues or questions, please open an issue on GitHub.

## 📄 License

MIT License - feel free to use this project for your own purposes.

## 👨‍💻 Author

Created for the Afghan cryptocurrency community.

---

**Made with ❤️ for Telegram Mini Apps**

> 💡 **Tip**: This is a demo/template. For production use, connect to real blockchain APIs and implement proper backend infrastructure.
