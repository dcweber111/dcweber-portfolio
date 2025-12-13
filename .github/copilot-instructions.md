# Copilot Instructions for dcweber-portfolio

## Project Overview
A **Next.js 15 portfolio website** built with TypeScript, React 19, and Material-UI (MUI). The frontend is a single client-side React app showcasing projects, skills, and contact information with dark/light mode toggle.

**Project Type**: Portfolio Web Application  
**Framework**: Next.js 15 with Turbopack  
**Key Stack**: React 19, TypeScript, MUI 7, Tailwind CSS 4, Emotion  
**Entry Point**: `/frontend/app/page.tsx` (1100+ line client component)

## Architecture & Key Patterns

### Structure
- **Single Page Application**: All content in `/app/page.tsx` with client-side navigation
- **Monorepo Root**: Only `/frontend` directory contains the application
- **Styling**: Hybrid approach using Tailwind CSS + MUI components + Emotion (via MUI)
- **CSS Variables**: Global dark/light mode via `--background`, `--foreground` in `globals.css`

### Critical Pattern: Client-Side Component
The entire page is marked `"use client"` because:
- Uses React hooks (useState, useEffect)
- Implements dark/light mode toggle with system preference detection
- Requires client-side interactivity (smooth scrolling, form handling)

**Never convert this to server-side rendering** - the theme toggle and navigation rely on client state.

### Component Composition (within page.tsx)
Large monolithic component organized into logical sections:
- Navigation bar (AppBar with theme toggle)
- Hero section (image, introduction)
- About section
- Projects showcase (MUI Cards with responsive Grid)
- Skills section
- Contact form (TextField components)
- Footer

**Pattern**: Uses MUI's `useMediaQuery` hook for responsive behavior instead of CSS media queries.

### Theme Management
- MUI `createTheme()` creates dark/light theme objects
- `ThemeProvider` wraps all MUI components
- System preference auto-detection: `useMediaQuery("(prefers-color-scheme: dark)")`
- Manual toggle stored in component state

## Development Workflow

### Essential Commands (run from `/frontend` directory)
```bash
npm run dev        # Start dev server with Turbopack on http://localhost:3000
npm run build      # Production build
npm run start      # Run production build locally
npm run lint       # Run ESLint (extends next/core-web-vitals + next/typescript)
```

### Dependencies to Know
- **MUI**: All UI components (Button, Card, TextField, etc.)
- **react-icons**: Social media icons (FaGithub, FaLinkedin, FaTwitter, HiOutlineMail)
- **Emotion**: CSS-in-JS via MUI internals (@emotion/react, @emotion/styled)
- **Tailwind CSS 4**: Available but currently minimal CSS (`globals.css` imports it)

### Linting & Code Style
- ESLint config extends Next.js recommended rules
- Ignores: `node_modules/`, `.next/`, `out/`, `build/`, `next-env.d.ts`
- TypeScript strict mode enabled

## Important Constraints & Decisions

### Why Everything is in page.tsx
- Avoids over-engineering a simple portfolio
- Single scroll-to-section navigation model
- Monolithic approach is intentional for this use case

### Styling Approach
- Tailwind CSS is installed but **MUI components are primary**
- Don't mix Tailwind utility classes with MUI components (causes conflicts)
- Use MUI's `sx` prop for component-level styling: `<Box sx={{ mt: 2 }}>`
- For global styles, update `globals.css` (currently minimal)

### Responsive Design
- MUI `Grid` component (imported as `MuiGrid`) for layouts
- `useMediaQuery` hook for conditional rendering
- Don't rely on CSS media queries; use MUI's responsive system

### Icons
- Import only what you need from `react-icons/fa`, `react-icons/hi`, `react-icons/io5`
- Icons are used for social links (GitHub, LinkedIn, Twitter) and theme toggle

## External Integration Points

### No Backend
This is a **frontend-only** portfolio. Any future contact form or email integration would require:
- External service (e.g., Formspree, EmailJS)
- Environment variables for API keys
- Form submission handler in page.tsx

### Image Handling
- Uses Next.js `Image` component for optimization
- Requires `/public` directory for static assets
- Currently no images configured; update `Image` src paths when adding portfolio images

## Common Tasks

### Add a New Project
1. Extend the `projects` array in page.tsx
2. Each project needs: title, description, image URL, technologies array, links
3. Projects render via `Map()` within MUI Grid layout

### Update Skills
Find the skills section in page.tsx and modify the array structure (category, skill name)

### Adjust Theme Colors
Modify the theme objects created by `createTheme()` in page.tsx (darkTheme, lightTheme)

### Add Social Link
Add icon import from react-icons, update social links array with URL and icon component

## TypeScript Notes
- Strict mode enabled in `tsconfig.json`
- Path alias configured: `@/*` maps to `/frontend/` root
- No component library types needed; MUI provides full types

## Deployment Considerations
- Build: `npm run build` (bundles with Turbopack)
- Output goes to `.next/` directory
- Can be deployed to Vercel (Next.js native) or any Node.js host
