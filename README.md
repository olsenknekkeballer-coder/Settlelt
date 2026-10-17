# SettleIt

A responsive event-planning dashboard starter built with React, TypeScript, Vite, and Cloudflare Workers.

## Included
- Responsive white/light interface
- Create plans with dates, times, locations, descriptions, and colours
- Plan overview, RSVP choices, tasks, and notes
- Calendar view and search
- Browser-local saving with `localStorage`
- Cloudflare Workers static asset deployment configuration

## Run locally
Install Node.js 20 or newer, then run:

```bash
npm install
npm run dev
```

## Deploy to Cloudflare Workers
1. Push this project to a GitHub repository.
2. In Cloudflare, open **Workers & Pages** and create a Worker.
3. Connect your GitHub repository and choose the Vite build settings:
   - Build command: `npm run build`
   - Build output directory: `dist`
4. Deploy. The included `wrangler.jsonc` is also configured for Wrangler CLI deployments.

## Current limitation
This starter saves plans in the current browser only. It does not yet have shared accounts, invitations, or a database. To make plans available across devices and to invited friends, connect a Supabase project and add database tables plus Row Level Security policies. Never put a Supabase service-role key in browser code.

## Logo
Put the SettleIt logo in `public/` and update `index.html` with a favicon link when you have the final image file.
