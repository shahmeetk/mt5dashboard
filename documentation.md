
# MT5 Trading Platform Documentation

## System Overview
This application is a web-based trading platform that integrates with MetaTrader 5 (MT5), providing account management and alert configuration capabilities.

### Tech Stack
- Frontend: React with TypeScript
- Backend: Node.js/Express
- Database: PostgreSQL with Drizzle ORM
- Authentication: Firebase
- Real-time Updates: WebSocket
- UI Framework: Tailwind CSS with Shadcn/UI components

## Core Features

### 1. Authentication System
- Firebase-based authentication
- Protected routes
- Session management
- User role management (Admin/Regular users)

### 2. MT5 Account Management
- Create and manage MT5 trading accounts
- View account summaries
- Monitor connection status
- Track open positions
- Real-time account updates via WebSocket

### 3. Alert Configuration
- Create custom trading alerts
- Configure alert parameters
- Real-time alert notifications
- Alert history tracking

### 4. Admin Dashboard
- User management
- System monitoring
- Account oversight
- Alert management

## Technical Implementation

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
├── routes.ts       # API endpoints
├── mt5-service.ts  # MT5 integration
├── auth.ts         # Authentication
└── db.ts          # Database operations
```

### Key Dependencies
- @tanstack/react-query: API state management
- wouter: Routing
- shadcn/ui: UI components
- express: Backend server
- drizzle-orm: Database ORM
- firebase: Authentication
- socket.io: Real-time updates

## Environment Configuration

Required environment variables:
```
DATABASE_URL=postgres://...
FIREBASE_API_KEY=your_api_key
FIREBASE_AUTH_DOMAIN=your_domain
FIREBASE_PROJECT_ID=your_project_id
MT5_API_ENDPOINT=your_mt5_endpoint
```

## Setup Instructions

1. Clone repository
2. Install dependencies: `npm install`
3. Configure environment variables
4. Run development server: `npm run dev`

## Development Workflow

1. Frontend development (port 5000)
2. Backend API (port 5000)
3. WebSocket connection for real-time updates
4. Database migrations with Drizzle

## Deployment

The application is configured to deploy on Replit with:
- Build command: `npm run build`
- Run command: `npm start`
- Port configuration: 5000

## Error Handling

- Firebase authentication errors
- MT5 connection issues
- Database transaction failures
- WebSocket disconnections

## Security Considerations

1. Protected routes
2. API authentication
3. Environment variables
4. Database security
5. WebSocket authentication

## Future Enhancements

1. Additional trading features
2. Enhanced alert system
3. Mobile responsiveness
4. Performance optimizations
5. Additional MT5 integrations

## Troubleshooting

Common issues and solutions:
1. Authentication failures
2. MT5 connection issues
3. Real-time update delays
4. Database connectivity problems

## API Documentation

### Authentication Endpoints
- POST /api/auth/login
- POST /api/auth/logout
- GET /api/auth/user

### MT5 Endpoints
- GET /api/mt5-accounts
- POST /api/mt5-accounts
- PATCH /api/mt5-accounts/:id
- DELETE /api/mt5-accounts/:id

### Alert Endpoints
- GET /api/alerts
- POST /api/alerts
- PATCH /api/alerts/:id
- DELETE /api/alerts/:id

## WebSocket Events
- account_update
- alert_triggered
- connection_status
- error_notification
