# Project Structure Documentation

## Root Directory
```
├── .git/                  # Git version control directory
├── .expo/                 # Expo configuration directory
├── .bolt/                 # Bolt configuration directory
├── assets/               # Static assets directory
├── dist/                 # Distribution/build output directory
├── src/                  # Source code directory
├── App.tsx              # Main application component
├── app.json             # Application configuration
├── babel.config.js      # Babel configuration
├── eas.json             # EAS (Expo Application Services) configuration
├── nativescript.config.ts # NativeScript configuration
├── package.json         # Project dependencies and scripts
├── package-lock.json    # Locked project dependencies
├── project.json         # Project configuration
├── references.d.ts      # TypeScript references
├── tailwind.config.js   # Tailwind CSS configuration
├── tsconfig.json        # TypeScript configuration
└── webpack.config.js    # Webpack configuration
```

## Source Directory (`src/`)
```
src/
├── api/                 # API integration and services
├── auth/               # Authentication related code
├── components/         # Reusable UI components
├── contexts/           # React Context providers
├── hooks/              # Custom React hooks
├── providers/          # Application providers
├── screens/            # Screen components
├── theme/              # Theme configuration and styles
├── utils/              # Utility functions
├── app.css             # Global CSS styles
├── app.ts              # Application entry point
├── NavigationParamList.ts # Navigation type definitions
└── types.ts            # TypeScript type definitions
```

## Key Files and Their Purposes

### Configuration Files
- `app.json`: Contains application metadata and configuration
- `babel.config.js`: Babel transpiler configuration
- `eas.json`: Expo Application Services configuration
- `nativescript.config.ts`: NativeScript framework configuration
- `tailwind.config.js`: Tailwind CSS styling configuration
- `tsconfig.json`: TypeScript compiler configuration
- `webpack.config.js`: Webpack bundler configuration

### Source Code Organization
- `src/api/`: API integration, services, and data fetching logic
- `src/auth/`: Authentication, authorization, and user management
- `src/components/`: Reusable UI components
- `src/contexts/`: React Context providers for state management
- `src/hooks/`: Custom React hooks for shared logic
- `src/providers/`: Application-wide providers
- `src/screens/`: Screen components for different routes/pages
- `src/theme/`: Theme configuration, styling, and design system
- `src/utils/`: Utility functions and helper methods

### Type Definitions
- `src/types.ts`: Global TypeScript type definitions
- `src/NavigationParamList.ts`: Navigation-related type definitions

## Development Guidelines

1. **Component Organization**
   - Place reusable components in `src/components/`
   - Screen-specific components should be in `src/screens/`
   - Keep components modular and focused on a single responsibility

2. **State Management**
   - Use React Context for global state (`src/contexts/`)
   - Implement custom hooks for shared logic (`src/hooks/`)

3. **Styling**
   - Use Tailwind CSS for styling (configured in `tailwind.config.js`)
   - Global styles are defined in `src/app.css`

4. **Type Safety**
   - Maintain type definitions in `src/types.ts`
   - Use TypeScript for all new code
   - Keep navigation types in `NavigationParamList.ts`

5. **API Integration**
   - API-related code should be organized in `src/api/`
   - Keep API calls and data fetching logic separate from components

## Build and Distribution
- Build output is generated in the `dist/` directory
- Static assets are stored in `assets/`
- Use `npm` or `yarn` for package management
- Configuration for different environments is managed through respective config files 