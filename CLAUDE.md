# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands
- **Development server:** `npm start` or `ng serve`
- **Build:** `npm run build` or `ng build`
- **Unit Tests:** `npm test` or `ng test` (Powered by Vitest)
- **End-to-End Tests:** `ng e2e`
- **Scaffolding:** `ng generate component <name>`
- **Formatting:** Prettier is configured for the project.

## Architecture & Structure
This is a modern Angular (v21+) application utilizing standalone components and reactive state management.

### Project Structure
- `src/app/components`: UI components (e.g., Hero, Details, RSVP, Footer)
- `src/app/services`: API and business logic
- `src/app/interfaces`: Type definitions and data models
- `src/app/constants`: Static event-related configurations

### Key Conventions
- **Standalone Components:** Use standalone components throughout; avoid `NgModules`.
- **Reactivity:** Prefer `signal` for reactive state management.
- **Service-Oriented Logic:** Keep components lean by moving business logic and data fetching into services.
- **Styling:** Use SCSS for component and global styles.
- **Networking:** HTTP requests are handled via `provideHttpClient()` in `app.config.ts` and encapsulated within services.
