# Forex Trading Platform - Replit Project

## Overview
This is a full-stack forex trading platform built with React, Express.js, and TypeScript. The application provides real-time market data, trading signals, educational content, and news for forex traders. It features a modern responsive UI built with shadcn/ui components and Tailwind CSS.

## System Architecture

### Frontend Architecture
- **Framework**: React 18 with TypeScript
- **UI Library**: shadcn/ui components with Radix UI primitives
- **Styling**: Tailwind CSS with custom design tokens
- **State Management**: TanStack Query for server state management
- **Routing**: Wouter for client-side routing
- **Charts**: Recharts for trading data visualization
- **Build Tool**: Vite for fast development and optimized builds

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **Database Provider**: Neon Database (serverless PostgreSQL)
- **API Style**: RESTful JSON API
- **Session Management**: Express sessions with PostgreSQL storage
- **Development**: Hot module replacement with Vite integration

### Key Components

#### Data Models
- **Users**: User authentication and profile management
- **Market Data**: Real-time forex currency pair information (prices, spreads, changes)
- **Trading Signals**: Buy/sell/hold recommendations with entry prices
- **News Articles**: Market news and analysis content
- **Educational Content**: Trading tutorials and learning materials

#### API Endpoints
- `GET /api/market-data` - Real-time forex market data
- `GET /api/trading-signals` - Trading recommendations
- `GET /api/news` - Latest market news articles
- `GET /api/education` - Educational content and tutorials
- `POST /api/contact` - Contact form submissions

#### UI Components
- **Market Data Table**: Real-time price display with auto-refresh
- **Trading Chart**: Interactive price charts using Recharts
- **Trading Signals**: Buy/sell recommendations display
- **News Section**: Latest market news with categories
- **Education Section**: Learning materials and tutorials
- **Contact Form**: Lead generation and customer inquiries

## Data Flow

1. **Real-time Market Data**: Frontend polls `/api/market-data` every 5 seconds for live price updates
2. **Trading Signals**: Fetched every 30 seconds to display current recommendations
3. **Static Content**: News and educational content loaded on page load
4. **Contact Forms**: Form submissions sent to `/api/contact` endpoint
5. **Error Handling**: Comprehensive error boundaries and toast notifications

## External Dependencies

### Frontend Dependencies
- React ecosystem (React, React DOM, React Router via Wouter)
- UI components (Radix UI primitives, shadcn/ui, Lucide icons)
- Data visualization (Recharts, Embla Carousel)
- Form handling (React Hook Form, Zod validation)
- State management (TanStack Query)
- Utilities (date-fns, clsx, class-variance-authority)

### Backend Dependencies
- Express.js server framework
- Database (Drizzle ORM, Neon Database client)
- Session management (connect-pg-simple)
- Development tools (tsx, esbuild for production builds)

### Development Tools
- TypeScript for type safety
- Tailwind CSS for styling
- PostCSS for CSS processing
- Vite for build tooling and development server
- Replit-specific plugins for development environment

## Deployment Strategy

### Development Environment
- Uses Vite dev server with hot module replacement
- Express server runs on Node.js with tsx for TypeScript execution
- Database migrations handled by Drizzle Kit
- Replit-specific configurations for cloud development

### Production Build
- Frontend built with Vite to static assets
- Backend compiled with esbuild to ESM modules
- Single Node.js process serves both API and static files
- Environment variables for database connection and configuration

### Database Strategy
- PostgreSQL database hosted on Neon (serverless)
- Drizzle ORM for type-safe database operations
- Migrations managed through Drizzle Kit
- Connection pooling handled by Neon's serverless architecture

## User Preferences

Preferred communication style: Simple, everyday language.

## Changelog

Changelog:
- July 07, 2025. Initial setup