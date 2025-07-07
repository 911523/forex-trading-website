# Forex Trading Platform

A professional forex trading platform with real-time market data, trading signals, educational content, and news. Built with React, Express.js, and TypeScript.

## Features

- **Real-time Market Data**: Live forex rates with 5-second updates
- **Trading Signals**: Buy/sell/hold recommendations with entry prices
- **Interactive Charts**: EUR/USD price visualization using Recharts
- **Educational Content**: Trading tutorials and learning materials
- **Market News**: Latest forex market developments
- **Contact Form**: Lead generation and customer inquiries
- **Professional Design**: Modern UI inspired by FastBull

## Tech Stack

### Frontend
- React 18 with TypeScript
- shadcn/ui components with Radix UI
- Tailwind CSS for styling
- TanStack Query for state management
- Wouter for routing
- Recharts for data visualization

### Backend
- Express.js with TypeScript
- In-memory storage for demo purposes
- RESTful API design
- Real-time data updates

## Getting Started

### Prerequisites
- Node.js 20 or higher
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone <your-repo-url>
cd forex-trading-platform
```

2. Install dependencies
```bash
npm install
```

3. Start the development server
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## API Endpoints

- `GET /api/market-data` - Real-time forex market data
- `GET /api/trading-signals` - Trading recommendations
- `GET /api/news` - Latest market news articles
- `GET /api/education` - Educational content and tutorials
- `POST /api/contact` - Contact form submissions

## Deployment

### Free Hosting Options

#### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your GitHub repository to Vercel
3. Deploy automatically with zero configuration

#### Netlify
1. Build the project: `npm run build`
2. Deploy the `dist` folder to Netlify

#### Railway
1. Connect your GitHub repository
2. Deploy with automatic builds

## Project Structure

```
├── client/                 # Frontend React application
│   ├── src/
│   │   ├── components/     # Reusable UI components
│   │   ├── pages/         # Application pages
│   │   ├── hooks/         # Custom React hooks
│   │   └── lib/           # Utility functions
├── server/                # Backend Express application
│   ├── index.ts          # Main server file
│   ├── routes.ts         # API routes
│   └── storage.ts        # Data storage layer
├── shared/               # Shared types and schemas
└── README.md
```

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source and available under the MIT License.

## Support

For support and questions, please contact us through the website contact form or email support@forexpro.com.

---

**Disclaimer**: Trading involves risk and may not be suitable for all investors. This platform is for educational and demonstration purposes.