# YouTube Video Metadata Extractor

## Overview

This is a YouTube video metadata extraction application built with React (frontend) and Express.js (backend). The application allows users to input YouTube video URLs and extract key metadata including title, thumbnail, duration, and other video information. The interface is primarily in Arabic, designed for Arabic-speaking users who want to quickly access YouTube video metadata.

## User Preferences

Preferred communication style: Simple, everyday language.
Image quality: User prefers highest quality thumbnails (Full HD 1920x1080) with direct download functionality.

## System Architecture

### Frontend Architecture
- **Framework**: React with TypeScript using Vite as the build tool
- **UI Library**: Shadcn/UI components built on Radix UI primitives
- **Styling**: Tailwind CSS with custom CSS variables for theming
- **State Management**: TanStack Query (React Query) for server state management
- **Routing**: Wouter for lightweight client-side routing
- **Form Handling**: React Hook Form with Zod validation
- **Internationalization**: Arabic language support with RTL (right-to-left) text direction

### Backend Architecture
- **Framework**: Express.js with TypeScript
- **Database ORM**: Drizzle ORM configured for PostgreSQL
- **Validation**: Zod schemas for request/response validation
- **Development**: Hot reload with tsx and Vite integration
- **Data Storage**: In-memory storage implementation with interface for future database integration

### Data Models
- **Users**: Basic user entity with username and password
- **Video Metadata**: Stores extracted YouTube video information including:
  - Video ID (extracted from YouTube URLs)
  - Title, thumbnail URL, duration
  - Duration in seconds for programmatic use
  - Original URL for reference

### API Design
- **RESTful endpoints**: Clean API structure with `/api` prefix
- **Video extraction endpoint**: POST `/api/extract-video` accepts YouTube URLs and returns metadata
- **Error handling**: Centralized error handling with Arabic error messages
- **Request logging**: Middleware for API request logging and performance monitoring

### Development Environment
- **Monorepo structure**: Shared TypeScript schemas between frontend and backend
- **Build process**: Separate build processes for client (Vite) and server (esbuild)
- **Development server**: Integrated Vite dev server with Express backend
- **Type safety**: Full TypeScript coverage with shared types via `@shared` alias

## External Dependencies

### Core Framework Dependencies
- **React ecosystem**: React, React DOM, React Hook Form, TanStack Query
- **Backend**: Express.js, Node.js with TypeScript support
- **Build tools**: Vite (frontend), esbuild (backend), tsx (development)

### Database and ORM
- **Drizzle ORM**: Modern TypeScript ORM for PostgreSQL
- **Neon Database**: Serverless PostgreSQL database (@neondatabase/serverless)
- **Database connection**: PostgreSQL with connection pooling support

### UI and Styling
- **Shadcn/UI**: Complete component library built on Radix UI
- **Radix UI**: Accessible component primitives (dialogs, forms, navigation, etc.)
- **Tailwind CSS**: Utility-first CSS framework with custom design system
- **Lucide React**: Icon library for consistent iconography

### Development and Quality
- **TypeScript**: Full type safety across the application
- **Zod**: Runtime type validation and schema definition
- **PostCSS**: CSS processing with Tailwind and Autoprefixer
- **Date-fns**: Date manipulation library

### Replit Integration
- **Replit-specific plugins**: Development banner, cartographer, runtime error overlay
- **Environment**: Optimized for Replit's development environment

The application uses a modern tech stack optimized for developer experience with full TypeScript support, component-based UI architecture, and clean separation between frontend and backend concerns.