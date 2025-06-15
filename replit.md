# خردة (Khurda) - Marketplace for Used Items

## Overview

This is a full-stack web application that serves as a marketplace for buying and selling used items. "Khurda" means "junk" or "scrap" in Arabic, allowing users to sell or give away anything they no longer need instead of throwing it away. The platform targets people moving homes, decluttering, or looking for budget-friendly deals.

## System Architecture

### Frontend Architecture
- **React 18** with TypeScript for the UI framework
- **Tailwind CSS** with shadcn/ui components for modern, responsive design
- **Zustand** for client-side state management
- **TanStack Query** for server state management and caching
- **Vite** as the build tool and development server
- **RTL (Right-to-Left)** support for Arabic language
- **Cairo font** for beautiful Arabic typography

### Backend Architecture
- **Express.js** server for API endpoints and static file serving
- **TypeScript** for type safety across the entire stack
- **Drizzle ORM** with PostgreSQL for database operations
- **Session-based authentication** ready for implementation
- **RESTful API** structure with `/api` prefix for all endpoints

### UI/UX Design
- **Modern gradient-based design** with emerald/green color scheme
- **Responsive design** supporting desktop, tablet, and mobile devices
- **Arabic-first interface** with proper RTL text alignment
- **Modern card-based layouts** with hover effects and shadows
- **Accessibility features** including proper contrast and focus states

## Key Components

### Marketplace Core Features
- **Item Listings**: Users can post items for sale with images, descriptions, and pricing
- **Category System**: 9 main categories including electronics, furniture, clothing, books, etc.
- **Search & Filter**: Real-time search with category filtering capabilities
- **User Profiles**: Complete user management with avatars and contact information
- **Favorites System**: Users can save items to their favorites list

### State Management
- **Marketplace Store**: Manages items, categories, search, and user state
- **Local Storage**: Persistent favorites and user preferences
- **Real-time Updates**: Dynamic filtering and search results

### User Interface Components
- **Modern Header**: Gradient design with search, notifications, and user controls
- **Category Sidebar**: Interactive category filter with item counts
- **Item Cards**: Modern card design with images, pricing, and seller info
- **Mobile-First Design**: Fully responsive layout for all device sizes

### Core Functionality
- **Item Management**: Add, edit, delete, and view item listings
- **Communication**: Direct messaging between buyers and sellers
- **Location-Based**: Items show location information for local transactions
- **Status Tracking**: Items can be active, sold, or reserved

## Data Flow

1. **User Interaction**: Browse categories, search items, and interact with listings
2. **State Management**: Zustand stores handle real-time filtering and updates
3. **UI Updates**: React components re-render based on state changes
4. **Local Storage**: Favorites and preferences persist across sessions
5. **API Integration**: Ready for backend communication for item CRUD operations
6. **Responsive Updates**: Dynamic category counts and search results

## External Dependencies

### Core Frameworks
- **React Ecosystem**: react, react-dom, @types/react
- **Three.js Ecosystem**: three, @react-three/fiber, @react-three/drei, @react-three/postprocessing
- **UI Library**: All Radix UI components via shadcn/ui implementation

### Development Tools
- **TypeScript**: Full type safety across frontend and backend
- **Vite**: Fast development server with HMR and optimized builds
- **Tailwind CSS**: Utility-first styling with custom design system
- **PostCSS**: CSS post-processing with autoprefixer

### Backend Infrastructure
- **Database**: @neondatabase/serverless for PostgreSQL hosting
- **ORM**: drizzle-orm with drizzle-kit for schema management
- **Session Management**: connect-pg-simple for PostgreSQL session storage

## Deployment Strategy

### Build Process
- **Frontend**: Vite builds optimized static assets to `dist/public`
- **Backend**: esbuild bundles server code to `dist/index.js`
- **Assets**: 3D models, textures, and audio files served statically

### Production Configuration
- **Environment**: NODE_ENV=production for server optimizations
- **Database**: DATABASE_URL environment variable for PostgreSQL connection
- **Static Serving**: Express serves built frontend from dist/public
- **Port Configuration**: Configurable port with fallback to 5000

### Replit Deployment
- **Autoscale**: Configured for automatic scaling based on demand
- **Build Command**: `npm run build` compiles both frontend and backend
- **Start Command**: `npm run start` runs production server
- **Development**: `npm run dev` with hot reload for development

## Changelog

- June 15, 2025. Initial setup

## User Preferences

Preferred communication style: Simple, everyday language.