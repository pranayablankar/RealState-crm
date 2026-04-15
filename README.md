# RealState CRM

Real estate plot CRM application built with React, Vite, TypeScript, shadcn/ui, Tailwind CSS, React Router, Zustand, and Supabase backend.

## Features
- **Dashboard** with key metrics
- **Leads Management**: Add, view, import leads
- **Plots Management**: Track real estate plots
- **Agents Management**
- **Activities & Follow-ups**
- **Call History & Reports**
- **Settings**: Lead sources/status, user management, notifications, integrations
- Responsive design with mobile support
- Supabase integration for auth, database, functions (webhooks for WhatsApp/FB/Google)

## Quick Start (Local Development)

1. **Install dependencies:**
   ```bash
   npm install
   ```

2. **Start development server:**
   ```bash
   npm run dev
   ```
   Open [http://localhost:5173](http://localhost:5173)

3. **Build for production:**
   ```bash
   npm run build
   ```

## Supabase Setup
1. Create Supabase project
2. Run migrations: `supabase db push` or apply SQL files
3. Deploy Edge Functions: `supabase functions deploy`
4. Update `src/integrations/supabase/client.ts` with your Supabase URL & anon key
5. Seed data if needed: `supabase functions deploy seed-users`

## Project Structure
```
src/
├── components/     # UI components (shadcn/ui)
├── contexts/       # Auth context
├── hooks/          # Custom hooks
├── pages/          # Route pages (Dashboard, Leads, Plots, etc.)
├── store/          # Zustand stores
└── integrations/   # Supabase client
supabase/           # Functions & migrations
```

## Scripts
- `npm run dev` - Start dev server
- `npm run build` - Build production
- `npm run lint` - Lint code
- `npm run test` - Run tests

## Tech Stack
![React](https://img.shields.io/badge/React-18-blue)
![Vite](https://img.shields.io/badge/Vite-5-orange)
![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4-green)
![Supabase](https://img.shields.io/badge/Supabase-2.45-purple)
![shadcn/ui](https://img.shields.io/badge/shadcn--ui-orange)

## Deployment
- Frontend: Vercel/Netlify/Vite Preview
- Backend: Supabase (PostgreSQL + Edge Functions)

---

**Live Demo:** [Coming soon]
**Backend:** Supabase

Built for real estate lead & plot management.
