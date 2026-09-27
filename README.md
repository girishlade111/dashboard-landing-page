# FlowAI — Dashboard Landing Page

A bright, modern marketing landing page for **FlowAI**, an AI-powered project-planning product ("Smarter Project Planning — Keep Your Team Aligned in Minutes"). Includes a gradient hero with dashboard preview mockup, features, how-it-works, and pricing sections, plus client-side login/signup pages.

> **Built by Girish Lade** — more free tools at [ladestack.in](https://ladestack.in)

## Features

- **Hero** — gradient + grid backdrop, headline, CTA, and dashboard preview mockup
- **Features section** — product capability cards with icons
- **How It Works** — step-by-step walkthrough section
- **Pricing section** — plan tiers and pricing cards
- **Login / Signup pages** — client-side forms with toast feedback (demo only, no backend)
- **Sticky navbar** — navigation with theme provider
- **Light, playful design** — rose/orange gradient palette, rounded cards
- **Responsive** — mobile-first Tailwind layouts

## Tech Stack

- **Next.js 15** (App Router, static export) + **React 19** + **TypeScript**
- **Tailwind CSS** + **shadcn/ui** (Radix UI primitives)
- **next-themes** for theming
- **lucide-react** icons, **@vercel/analytics**

## Quick Start

```bash
# install dependencies
npm install

# run the dev server
npm run dev
# open http://localhost:3000

# production build (static export to ./out)
npm run build

# serve the static build
npx serve out
```

## Project Structure

```
app/                        # Next.js App Router
  page.tsx                  # Landing page (hero + sections)
  login/page.tsx            # Client-side login (demo)
  signup/page.tsx           # Client-side signup (demo)
  layout.tsx / globals.css
components/
  flowai/
    navbar.tsx / hero.tsx
    dashboard-preview.tsx
    sections/               # features, how-it-works, pricing
  ui/                       # shadcn/ui primitives
  theme-provider.tsx
hooks/use-toast.ts          # Toast hook
lib/utils.ts
public/                     # Static assets
styles/
```

## Environment Variables

None — pure static landing page; the login/signup forms are client-side demos with no backend or secrets.

## Deployment

Static site. Build with `npm run build` (configured with `output: 'export'`, images unoptimized) and deploy the `out/` directory to any static host — GitHub Pages, Cloudflare Pages, Netlify, or Vercel.

## License

Free to use and modify.
