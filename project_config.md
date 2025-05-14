# Project Configuration (LTM)

*This file contains the stable, long-term context for the project.*
*It should be updated infrequently, primarily when core goals, tech, or patterns change.*

---

## Core Goal

*(Define the primary objective and purpose of this project here. E.g., "Create a web application for managing personal tasks...")*

---

## Tech Stack

*   **Framework:** Next.js ≥15.2.3 (Full-stack, Pages Router)
*   **Language:** TypeScript
*   **Styling:** Tailwind CSS
*   **Database:** PostgreSQL (via Supabase)
*   **ORM:** Prisma
*   **Monitoring & Logging:** 
    *   HyperDX (Logging & Tracing)
    *   Sentry (Error Management)
*   **Testing:** Jest, React Testing Library
*   **Linting/Formatting:** ESLint, Prettier

---

## Critical Patterns & Conventions

*   **State Management:** Zustand for global state management
*   **Data Validation:** Zod for runtime type checking and validation
*   **Authentication:**
    *   Global middleware for route protection
    *   Server Actions must include authentication verification
*   **API Patterns:**
    *   Server Actions for all mutations (create, update, delete operations)
    *   API Routes for read operations and external service integrations
    *   up-fetch for all client-side fetch operations
*   **Error Handling:**
    *   Use `next-error` for consistent error handling across the application
    *   Implement error boundaries with `react-error-boundary`
    *   Custom `AppError` class for backend errors
    *   Error logging through Sentry
    *   Client-side error tracking with `@sentry/nextjs`
*   **Commit Messages:** Follow Conventional Commits format

---

## Key Constraints

*   **Browser Support:** Must support the last 2 versions of Chrome and Edge
*   **Deployment:** Vercel platform
*   **Performance:** Strict adherence to Core Web Vitals metrics

---

## Tokenization Settings

*   **Estimation Method:** Character-based
*   **Characters Per Token (Estimate):** 4
