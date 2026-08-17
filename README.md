## Hi, I'm Gabrielly 👋

**Full-Stack Developer** — React · Next.js · TypeScript · Node.js · Supabase
Currently Help Desk & QA Analyst at Cognizant.

🌎 **Native Portuguese & Spanish · English (working proficiency)**

🔧 **The Support Engineer Mindset:** My background in IT Support means I don't just patch symptoms. I trace bugs, read error logs, and I care about writing secure, maintainable code.

📫 gabiferreira101@gmail.com · [LinkedIn](https://www.linkedin.com/in/gabrielly-ferreira-619609113/)

---

### 🚀 Featured Projects

**[Desk Control](https://github.com/GabriellyFerreiraa/desk-control)** — [Live demo](https://tranquil-syrniki-a20c8e.netlify.app/)
Service desk management tool: role-based dashboards (Lead/Analyst), shift scheduling, absence approval workflow, all backed by Supabase Row Level Security.
> Authorization is enforced at the **database level** through Supabase Row Level Security, not in the UI — a Lead can't see Analyst-only data even by calling the API directly. Hiding buttons in the frontend is not access control.

`React` `TypeScript` `Supabase` `Tailwind`

**[TicketSense](https://github.com/GabriellyFerreiraa/ticketsense)** — [Live demo](https://ticketsense.netlify.app/)
AI-assisted support ticket triage — Gemini classifies category/urgency and suggests first diagnostic steps via a Supabase Edge Function, keeping the API key off the client entirely.
> The AI call runs inside a **Supabase Edge Function**, so the Gemini API key never touches the client bundle — a deliberate choice over the common shortcut of calling the API straight from the frontend, which exposes the key to anyone who opens DevTools.

`React` `TypeScript` `Supabase Edge Functions` `Gemini API`

**[Service Desk API](https://github.com/GabriellyFerreiraa/servicedesk-api)**
REST API built from scratch: JWT authentication, role-based access control (Admin/Agent/Requester) with roles in a dedicated table to prevent privilege escalation, integration tests and CI on GitHub Actions.
> Roles live in a **dedicated table**, not as a column on the user record — a deliberate security decision that prevents privilege escalation if the user row is ever compromised through mass-assignment.

`Node.js` `Express` `TypeScript` `PostgreSQL` `Prisma`

**[TicketSense (Next.js)](https://github.com/GabriellyFerreiraa/ticketsense-next)** — [Live demo](https://ticketsense-next.vercel.app)
The same AI triage product, rebuilt on Next.js 16 App Router to compare architectures.

> The Gemini call moved from a Supabase Edge Function to a **Route Handler**, and route protection moved from a client-side guard to **`proxy.ts`** — so a protected page's HTML is never generated for an unauthenticated visitor. Both versions keep the API key server-side; only the plumbing changes. [Full comparison in the README.](https://github.com/GabriellyFerreiraa/ticketsense-next#-why-two-versions)

`Next.js 16` `React 19` `TypeScript` `Supabase` `Gemini API`

[Payload CMS Demo](https://github.com/GabriellyFerreiraa/payload-cms-demo) — [Live demo](https://payload-cms-demo-sigma.vercel.app/)
Headless CMS running inside a Next.js App Router app: content model defined in TypeScript, authored in the Payload admin panel, stored in Postgres, rendered by Server Components.

Payload is a dependency of the app, not a service beside it — content is read through `payload.find()`, a direct database query on the server, so there's no API token in the render path and no network hop on every render. [Trade-offs against a hosted CMS in the README.](https://github.com/GabriellyFerreiraa/payload-cms-demo#-why-build-this)

`Next.js` `Payload CMS` `TypeScript` `PostgreSQL (Neon)` `Vercel`

---

### 🛠️ Stack

`React` · `Next.js` · `TypeScript` · `JavaScript` · `Tailwind CSS` · `Supabase (Postgres, Auth, RLS, Edge Functions)` · `Firebase` · `HTML/CSS`· `Node.js` · `Express` · `PostgreSQL` · `Prisma` · `Payload CMS`

### 💬 Ask me about
Debugging Row Level Security, connecting AI APIs to real apps without leaking keys, choosing where the server boundary goes in a Next.js app, or anything IT-support-turned-dev related.

