# Tax Genius AI

A modern React application built with Vite for intelligent tax assistance and calculations.

## Features

- Built with React 19 and Vite for fast development and optimal performance
- Styled with Tailwind CSS for responsive and modern UI
- Lucide React icons for beautiful iconography
- ESLint configuration for code quality
- Hot Module Replacement (HMR) for instant development feedback

## Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (version 18.0 or higher)
- **npm** (comes with Node.js) or **yarn**

You can check your versions by running:
```bash
node --version
npm --version
```

## Installation

1. **Clone the repository** (if not already done):
   ```bash
   git clone <repository-url>
   cd tax-genius-ai
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```
   
   Or if you prefer yarn:
   ```bash
   yarn install
   ```

## Getting Started

### Development Server

To start the development server with hot reload:

```bash
npm run dev
```

Or with yarn:
```bash
yarn dev
```

The application will be available at `http://localhost:5173`

### Build for Production

To build the application for production:

```bash
npm run build
```

The build artifacts will be stored in the `dist/` directory.

### Preview Production Build

To preview the production build locally:

```bash
npm run preview
```

### Linting

To run ESLint and check for code quality issues:

```bash
npm run lint
```

## Project Structure

```
tax-genius-ai/
├── public/                 # Static assets
├── src/                   # Source code
│   ├── components/        # React components
│   ├── pages/            # Page components
│   ├── styles/           # CSS/styling files
│   ├── utils/            # Utility functions
│   ├── App.jsx           # Main App component
│   └── main.jsx          # Application entry point
├── index.html            # HTML template
├── package.json          # Dependencies and scripts
├── vite.config.js        # Vite configuration
├── tailwind.config.js    # Tailwind CSS configuration
├── eslint.config.js      # ESLint configuration
└── README.md             # This file
```

## Configuration

### Tailwind CSS

The project is configured with Tailwind CSS. The configuration file is located at `tailwind.config.js`. You can customize the theme, add plugins, or modify the content paths as needed.

### Vite

Vite configuration is in `vite.config.js`. The current setup includes:
- React plugin for JSX support
- Hot Module Replacement (HMR)

### ESLint

ESLint is configured in `eslint.config.js` with:
- React hooks rules
- React refresh plugin
- Modern JavaScript support

## Deployment

### Build the Application

```bash
npm run build
```

### Deploy to Vercel

1. Install Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Deploy:
   ```bash
   vercel
   ```

### Deploy to Netlify

1. Build the application:
   ```bash
   npm run build
   ```

2. Drag and drop the `dist` folder to [Netlify Drop](https://app.netlify.com/drop)

### Deploy to GitHub Pages

1. Install gh-pages:
   ```bash
   npm install --save-dev gh-pages
   ```

2. Add to package.json scripts:
   ```json
   "predeploy": "npm run build",
   "deploy": "gh-pages -d dist"
   ```

3. Deploy:
   ```bash
   npm run deploy
   ```

## Development Tips

- **Hot Reload**: Save any file to see changes instantly in the browser
- **Component Development**: Create reusable components in the `src/components` directory
- **Styling**: Use Tailwind CSS classes for styling, or create custom CSS in the `src/styles` directory
- **Icons**: Lucide React is available for beautiful icons

## Dependencies

### Main Dependencies
- **React**: UI library
- **React DOM**: React renderer for web
- **Lucide React**: Icon library

### Development Dependencies
- **Vite**: Build tool and dev server
- **Tailwind CSS**: Utility-first CSS framework
- **ESLint**: Code linting
- **TypeScript types**: Type definitions for React

## Troubleshooting

### Common Issues

1. **Port already in use**:
   ```bash
   # Kill process using port 5173
   npx kill-port 5173
   # Or use a different port
   npm run dev -- --port 3000
   ```

2. **Dependencies issues**:
   ```bash
   # Clear npm cache
   npm cache clean --force
   # Delete node_modules and reinstall
   rm -rf node_modules package-lock.json
   npm install
   ```

3. **Build errors**:
   ```bash
   # Check for linting errors
   npm run lint
   # Clear Vite cache
   rm -rf node_modules/.vite
   ```

---

**Happy coding! 🎉**
