
# MT5 Trading Platform Project Requirements

## Project Overview

### Vision
A web-based trading platform that integrates with MetaTrader 5 (MT5) to provide real-time account monitoring, alert management, and position tracking capabilities.

### Core Objectives
1. Create a modern, responsive trading interface
2. Enable real-time MT5 account monitoring
3. Implement a robust alert system
4. Provide secure authentication and authorization
5. Support multiple MT5 accounts management

## Technical Architecture

### Frontend Stack
- React with TypeScript for UI
- Tailwind CSS with custom theme support (Light/Dark modes)
- Shadcn/UI for component library
- WebSocket for real-time updates
- React Query for state management

### Backend Stack
- Node.js/Express server
- PostgreSQL database with Drizzle ORM
- Firebase Authentication
- WebSocket server for real-time data
- MT5 integration service

## MVP Features

### 1. Authentication System
- Firebase-based user authentication
- Protected routes
- Session management
- Role-based access control (Admin/User)

### 2. MT5 Account Management
- Connect multiple MT5 accounts
- Real-time account status monitoring
- Balance and equity tracking
- Open positions overview
- Account performance metrics

### 3. Alert Configuration
- Custom alert creation
- Multiple alert types support
- Real-time alert notifications
- Alert history tracking
- Alert status management

### 4. Dashboard Features
- Account summary cards
- Real-time balance updates
- Position monitoring
- Performance charts
- Account health indicators

### 5. Admin Features
- User management
- System monitoring
- Account oversight
- Alert management
- Activity logging

## Security Requirements

1. Secure Authentication
   - Firebase authentication integration
   - JWT token management
   - Session handling
   - Password policies

2. Data Protection
   - Encrypted MT5 credentials
   - Secure WebSocket connections
   - Database encryption
   - API security measures

## User Experience Requirements

1. Interface Design
   - Clean, modern UI
   - Responsive layout
   - Dark/Light theme support
   - Mobile-friendly design

2. Real-time Updates
   - Instant balance updates
   - Live position tracking
   - Real-time alerts
   - Connection status indicators

## Implementation Guidelines

### Frontend Structure
```
client/src/
├── components/      # UI components
├── hooks/          # Custom React hooks
├── lib/            # Utility functions
└── pages/          # Route components
```

### Backend Structure
```
server/
├── routes/         # API endpoints
├── services/       # Business logic
├── models/         # Data models
└── utils/          # Helper functions
```

## Development Phases

### Phase 1: Core Infrastructure
- Basic authentication
- MT5 connection setup
- Database implementation
- WebSocket integration

### Phase 2: Account Management
- MT5 account integration
- Real-time data flow
- Position tracking
- Account monitoring

### Phase 3: Alert System
- Alert configuration
- Notification system
- Alert history
- Custom alert rules

### Phase 4: Advanced Features
- Admin dashboard
- Performance analytics
- Enhanced security
- Mobile optimization

## Technical Specifications

### API Endpoints
- Authentication routes
- MT5 account management
- Alert configuration
- User management
- System monitoring

### WebSocket Events
- Account updates
- Position changes
- Alert triggers
- Connection status
- System notifications

### Database Schema
- User accounts
- MT5 credentials
- Alert configurations
- Trading history
- System logs

## Deployment Specifications

### Environment
- Replit hosting
- Production port: 5000
- WebSocket port: 5000
- Database: PostgreSQL

### Configuration
- Environment variables
- Firebase credentials
- MT5 API settings
- Database connection
- WebSocket settings

## Future Enhancements
1. Advanced trading features
2. Enhanced analytics
3. Mobile application
4. API integrations
5. Additional broker support

