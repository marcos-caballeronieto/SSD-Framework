# Technical Stack Specification

## 1. Core Development Stack
*Define the primary tools for building the application.*
- **Frontend Framework:** [e.g., React 19 + Vite, Svelte 5, Next.js 16]
- **Language:** [e.g., TypeScript 5.x (Strict Mode)]
- **Styling:** [e.g., Tailwind CSS 4.0, Radix UI, Shadcn/ui]
- **State Management:** [e.g., Zustand, TanStack Query, Signals]

## 2. AI & Orchestration Layer (The AI-Native Core)
*Crucial for 2026. This defines how the agents interact with your code.*
- **Primary Model:** [e.g., Claude 3.7 Sonnet, Gemini 2.0 Ultra]
- **Orchestration Framework:** [e.g., Pydantic AI, LangChain, Custom MCP Hooks]
- **Vector Database (if applicable):** [e.g., Pinecone, Supabase Vector, Chroma]
- **Context Management:** [e.g., Long-context window (200k+), Local RAG, Context7 MCP (Real-time Docs)]

## 3. Data & Persistence
- **Database:** [e.g., PostgreSQL (Supabase), MongoDB, SQLite]
- **ORM / Query Builder:** [e.g., Prisma, Drizzle, Kysely]
- **Caching:** [e.g., Redis, Browser LocalStorage]

## 4. Testing & Quality Assurance
- **Unit Testing:** [e.g., Vitest, Jest]
- **E2E Testing:** [e.g., Playwright (Mandatory for SDD workflow)]
- **Linter / Formatter:** [e.g., Biome, ESLint + Prettier]

## 5. Infrastructure & Deployment
- **Hosting:** [e.g., Vercel, Netlify, Railway]
- **CI/CD:** [e.g., GitHub Actions]
- **Observability:** [e.g., LangSmith, Logfire, Sentry]

## 6. Development Constraints (The "No-Go" Zone)
*Strict rules to keep the agent from introducing technical debt.*
- **No External Assets:** All visual assets must be programmatic (SVG/CSS) or AI-generated via p5.js.
- **Dependency Limit:** Do not add new NPM packages without user approval.
- **Type Safety:** 100% TypeScript coverage. No use of `any` types.
- **Component Pattern:** [e.g., Use Functional Components and Hooks only].

## 7. Executable Commands
*Commands the agent can run in the terminal.*
- **Install:** `npm install`
- **Dev Server:** `npm run dev`
- **Build:** `npm run build`
- **Test:** `npm test` or `npx playwright test`