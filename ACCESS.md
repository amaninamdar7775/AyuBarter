# Access Instructions for AyuBarter Application

## Frontend Access

You can now access the AyuBarter frontend using either of the following URLs:

### Primary URL
- **http://localhost:3000** - Main access URL

### Alternative URL
- **http://127.0.0.1:3000** - IP-based access URL

## Backend/API Access

The backend APIs and Socket.IO server are accessible at:

### API Endpoints
- **http://localhost:3000/api/** - Main API base URL
- **http://127.0.0.1:3000/api/** - Alternative API access

### Socket.IO WebSocket
- **ws://localhost:3000/api/socketio** - Main WebSocket URL
- **ws://127.0.0.1:3000/api/socketio** - Alternative WebSocket URL

## Configuration Details

### Server Configuration
- **Hostname**: 0.0.0.0 (binds to all interfaces)
- **Port**: 3000
- **Environment**: Development

### CORS Configuration
- **Allowed Origins**: 
  - http://localhost:3000
  - http://127.0.0.1:3000
- **Allowed Methods**: GET, POST, PUT, DELETE, OPTIONS
- **Allowed Headers**: Content-Type, Authorization

## Features Available

### Frontend Features
- 🌿 Modern Ayurvedic e-commerce interface
- 🛒 HealthCart for product browsing
- 👨‍⚕️ Doctor consultation booking
- 🔄 Barter system for community exchange
- 👥 Community features
- 🧘 Wellness programs

### Backend Features
- 🔐 User authentication system
- 📦 Product management API
- 👨‍⚕️ Doctor consultation API
- 💬 Real-time messaging via Socket.IO
- 📊 Analytics and reporting
- 🗄️ Database integration with Prisma

## Development Commands

```bash
# Start development server
npm run dev

# Build for production
npm run build

# Start production server
npm start

# Run linting
npm run lint

# Database operations
npm run db:push
npm run db:generate
npm run db:migrate
```

## Troubleshooting

If you encounter any issues:

1. **Port already in use**: Make sure port 3000 is not being used by another application
2. **Page not loading**: Try both URLs:
   - http://localhost:3000
   - http://127.0.0.1:3000
3. **CORS issues**: The server is configured to allow both localhost:3000 and 127.0.0.1:3000
4. **Socket.IO connection**: Verify WebSocket connections using the provided URLs
5. **Server not responding**: Check if the development server is running with `npm run dev`

## Network Configuration

The application is configured to work on both:
- **localhost:3000** - Standard localhost access
- **127.0.0.1:3000** - IP-based access

Both URLs provide full access to all frontend and backend features. The server binds to 0.0.0.0 to ensure accessibility from all network interfaces.