# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands
- Install: `npm install`
- Dev server: `npm run dev` (starts at localhost:4321)
- Build: `npm run build` (outputs to ./dist/)
- Preview build: `npm run preview`
- Astro CLI: `npm run astro -- <command>` (e.g., astro add, astro check)

## Code Style
- **TypeScript**: Use strict typing with Astro's TypeScript configuration
- **Components**: 
  - React components use .tsx extension with functional component pattern
  - Astro components use .astro extension with frontmatter for imports
- **Tailwind**: Follow utility-first approach with custom theme values in tailwind.config.mjs
- **Naming**: Use camelCase for variables/functions, PascalCase for components
- **Imports**: Group imports by type (React, components, styles)
- **Formatting**: Follow existing indentation (2 spaces) and line breaks
- **Error Handling**: Use try/catch for async operations, null checks for optional values
- **Theme**: Support light/dark modes using theme-provider.tsx system

## Project Structure
- `/src/components`: Reusable UI components (.astro or .tsx)
- `/src/layouts`: Page layout templates
- `/src/pages`: Route-based page components
- `/src/styles`: Global CSS and Tailwind configuration