# sparkalhood-assignment-frontend

# AI Safety Incident Dashboard

A frontend interface to view and log hypothetical AI safety incidents, built for HumanChain.

## Features

- Display a list of AI safety incidents with title, severity, and reported date
- Filter incidents by severity (All, Low, Medium, High)
- Sort incidents by reported date (newest/oldest first)
- Expand incident details with a toggle
- Report new incidents with a form and basic validation
- Responsive design that works on all devices
- Modern UI with smooth animations and transitions

## Tech Stack

- React 18 with TypeScript
- Tailwind CSS for styling
- date-fns for date formatting
- Vite for build tooling

## Getting Started

### Prerequisites

- Node.js (v14.x or higher)
- npm or yarn

### Installation

1. Clone the repository
2. Install dependencies:

```bash
npm install
```

3. Start the development server:

```bash
npm run dev
```

4. Open your browser and navigate to the URL shown in your terminal (typically http://localhost:5173)

### Building for Production

```bash
npm run build
```

The built files will be in the `dist` directory.

## Design Decisions

### Component Structure
- Used a modular component architecture for better maintainability
- Each component has a single responsibility and is easily testable
- Shared types are centralized in a types directory

### State Management
- Utilized React's built-in useState for local state management
- Props drilling is minimized through thoughtful component composition
- State updates are handled through clear, type-safe functions

### Styling
- Implemented Tailwind CSS for rapid development and consistent design
- Custom utility classes for common patterns
- Responsive design with mobile-first approach
- Smooth animations and transitions for better UX
- Semantic color system for severity levels
- Accessible focus states and keyboard navigation

### User Experience
- Clear visual hierarchy and information architecture
- Immediate feedback for user actions
- Form validation with helpful error messages
- Smooth transitions and animations
- Responsive layout that works on all screen sizes

### Performance
- Lazy loading of incident details
- Optimized re-renders using proper React patterns
- Efficient sorting and filtering algorithms
- Minimal bundle size through proper code splitting

## Project Structure

```
src/
├── components/        # React components
├── types/            # TypeScript type definitions
├── data/            # Mock data and constants
├── App.tsx          # Main application component
└── main.tsx         # Application entry point
```

## Future Improvements

- Add search functionality
- Implement data persistence
- Add unit tests
- Add keyboard shortcuts
- Implement dark mode
- Add export functionality for incident reports
- Implement user authentication
- Add real-time updates
