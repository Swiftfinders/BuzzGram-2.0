# BuzzGram 2.0 Frontend

A modern, full-stack business discovery platform built with React, TypeScript, and Tailwind CSS.

## Tech Stack

- **React 18** - UI library
- **TypeScript** - Type safety
- **Vite** - Fast build tool and dev server
- **React Router** - Client-side routing
- **TanStack Query** - Data fetching and caching
- **Axios** - HTTP client
- **Tailwind CSS** - Utility-first styling
- **Dark Mode** - Full dark mode support

## Features

- Browse cities with beautiful image cards
- Filter businesses by category
- Search businesses by name or description
- View detailed business information
- Fully responsive design
- Dark/light mode toggle
- Production-ready code with TypeScript
- Error handling and loading states

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- npm or yarn

### Installation

\`\`\`bash
# Install dependencies
npm install
\`\`\`

### Development

\`\`\`bash
# Start the dev server (runs on http://localhost:5173)
npm run dev
\`\`\`

### Build

\`\`\`bash
# Build for production
npm run build
\`\`\`

### Preview

\`\`\`bash
# Preview production build
npm run preview
\`\`\`

## API Integration

The frontend connects to the BuzzGram 2.0 backend API:

- **Development**: \`http://localhost:3001\`
- **Production**: \`https://triumphant-abundance-production.up.railway.app\`

The API base URL is automatically selected based on the environment (development vs production).

## Project Structure

\`\`\`
frontend/
├── src/
│   ├── components/          # Reusable UI components
│   │   ├── Header.tsx       # Navigation header with dark mode toggle
│   │   ├── BusinessCard.tsx # Business listing card
│   │   ├── CityGrid.tsx     # Grid of city cards
│   │   ├── CategoryFilter.tsx # Category filter dropdown
│   │   └── LoadingSpinner.tsx # Loading indicator
│   ├── pages/               # Route pages
│   │   ├── HomePage.tsx     # City selection page
│   │   ├── CityPage.tsx     # Business listings for a city
│   │   └── BusinessDetail.tsx # Individual business details
│   ├── lib/                 # Utilities and configuration
│   │   ├── api.ts           # Axios client and API functions
│   │   └── queryClient.ts   # TanStack Query configuration
│   ├── types/               # TypeScript type definitions
│   │   └── index.ts         # Shared types
│   ├── App.tsx              # Main app component with routing
│   ├── main.tsx             # Application entry point
│   └── index.css            # Global styles and Tailwind imports
├── public/                  # Static assets
├── package.json             # Dependencies and scripts
├── vite.config.ts           # Vite configuration
├── tsconfig.json            # TypeScript configuration
├── tailwind.config.js       # Tailwind CSS configuration
└── postcss.config.js        # PostCSS configuration
\`\`\`

## Available Routes

- \`/\` - Home page (city selection)
- \`/city/:cityId\` - Businesses in a specific city
- \`/business/:id\` - Detailed business information

## Environment Variables

The app automatically detects the environment:
- In development mode, it uses \`http://localhost:3001\`
- In production mode, it uses the Railway deployment URL

## Dark Mode

Dark mode is implemented using Tailwind's dark mode class strategy. Users can toggle between light and dark themes using the button in the header. The preference is saved to localStorage.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

Private project for BuzzGram 2.0
