# System Monitor App - VS Code Setup Guide

## Quick Start

1. **Download all project files** from this cloud environment
2. **Extract to a local folder** on your machine
3. **Open the folder in VS Code**
4. **Run setup commands** below

## Setup Commands

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build

# Run tests
npm test
```

## Project Structure

```
system-monitor-app/
├── client/                 # React frontend
│   ├── components/        # UI components
│   │   ├── ui/           # Shadcn/ui components
│   │   ├── Charts.tsx    # Data visualization
│   │   ├── Layout.tsx    # Main layout with sidebar
│   │   └── RealTimeTracker.tsx
│   ├── contexts/         # React contexts
│   ├── hooks/           # Custom hooks
│   ├── pages/           # App pages/routes
│   ├── App.tsx          # Main app component
│   └── global.css       # Global styles
├── server/              # Express.js backend
│   ├── routes/         # API routes
│   └── index.ts        # Server entry
├── shared/             # Shared utilities
├── package.json        # Dependencies & scripts
└── tailwind.config.ts  # Tailwind configuration
```

## Development URLs

- **Development server**: http://localhost:5173
- **API endpoints**: http://localhost:5173/api/\*

## Key Features

- **System Monitoring**: CPU, memory, disk usage tracking
- **App Usage Analytics**: Screen time, app limits, focus modes
- **Real-time Tracking**: Live data updates and streaming
- **Data Visualization**: Interactive charts with Recharts
- **Dark/Light Theme**: Toggle with persistence
- **Responsive Design**: Mobile-friendly interface
- **Professional UI**: Microsoft-level presentation quality

## Technologies Used

- **Frontend**: React 18, TypeScript, Tailwind CSS
- **Backend**: Express.js, Node.js
- **UI Components**: Radix UI, Shadcn/ui
- **Charts**: Recharts
- **Icons**: Lucide React
- **Routing**: React Router 6
- **Build Tool**: Vite

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm test` - Run tests
- `npm run typecheck` - Type checking

## Environment Setup

No environment variables required for basic functionality. The app includes mock data for demonstration.

## Troubleshooting

1. **Port conflicts**: If port 5173 is busy, Vite will automatically use the next available port
2. **Dependencies**: Run `npm install` if you see import errors
3. **TypeScript errors**: Run `npm run typecheck` to check for type issues
4. **Build issues**: Clear node_modules and reinstall: `rm -rf node_modules package-lock.json && npm install`

## VS Code Extensions Recommended

- ES7+ React/Redux/React-Native snippets
- Tailwind CSS IntelliSense
- TypeScript Importer
- Auto Rename Tag
- Prettier - Code formatter
- ESLint

## File Export Instructions

To get all files locally:

1. Download/export all files from the cloud environment
2. Maintain the exact folder structure shown above
3. Ensure all hidden files (.gitignore, etc.) are included
4. Keep package.json and node_modules structure intact
