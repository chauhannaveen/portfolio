# Portfolio Website Spec

## Goal
Build a single-page portfolio website for a technical founder/developer who builds production-ready SaaS products fast using AI-assisted development. The site's job is to convert visitors (potential freelance/contract clients, mostly US-based) into booked calls or messages.

## Tech requirements
- Single HTML page (or a simple single-page Next.js/Angular app if that fits the existing stack better — otherwise plain HTML/CSS/vanilla JS is fine)
- No CMS, no backend needed
- Mobile-first responsive design — most traffic will come from phones (X/LinkedIn/Reddit links)
- Fast load, minimal dependencies
- Deploy-ready for Vercel or Netlify
- Clean, modern, developer-credible aesthetic — not generic Bootstrap-template look. Dark or light theme, good typography, generous whitespace. Should look like it was built by someone who builds good software, not stock template.

## Tone
Confident, direct, no fluff. Speaks to non-technical founders and small businesses who need a product built, not to other developers. Avoid jargon-heavy buzzwords.

## Page structure

### 1. Hero section
- Headline: "I build production-ready SaaS products in weeks, not months, using AI-assisted development."
- Subheadline: One or two lines establishing credibility — technical founder, full-stack (.NET, Angular, PostgreSQL), builds real products end-to-end, not just prototypes.
- Primary CTA button: "Book a call" (placeholder Calendly link — use `#` for now) or "Message me" (placeholder mailto: or contact link)

### 2. Case studies section (core of the page)
Repeatable card/block per project, most important project first. For each:
- Project name
- One-line description of the problem it solves
- Screenshot or placeholder image block (use a simple gray placeholder div with alt text if no image provided yet)
- Tech stack badges/tags
- Build time callout (bolded or highlighted — this is the key differentiator): e.g. "Built solo in X weeks"
- Live link button (if deployed) and/or GitHub link button (if public repo) — omit whichever doesn't apply

**Project 1: GhostRadar**
- One-liner: A job application transparency platform that crowdsources ghosting rates, response times, and candidate experience data for companies, helping job seekers know what to expect before they apply.
- Tech stack: .NET 8, Angular 18, PostgreSQL, EF Core, Google OAuth + Gmail API, SignalR (web push via VAPID), Stripe billing, PWA with offline sync, GitHub Actions CI/CD (Docker + GHCR)
- Build time: mention if known, e.g. "Built solo across several weeks, from architecture to a full production-ready stack including admin moderation panel, anti-spam detection, and automated billing."
- Live link: [ADD IF DEPLOYED — otherwise leave as GitHub/demo link placeholder]
- Notable detail to highlight: full end-to-end SaaS — auth, billing, real-time notifications, PWA, moderation, CI/CD — not just a UI prototype.

**Project 2: [FILL IN — product name]**
- One-liner: [describe the problem it solves]
- Tech stack: [list]
- Build time: [X weeks/days]
- Live link / GitHub link: [add]

**Project 3: [FILL IN — product name]**
- One-liner: [describe the problem it solves]
- Tech stack: [list]
- Build time: [X weeks/days]
- Live link / GitHub link: [add]

**Project 4 (optional): [FILL IN — product name]**
- Same structure as above.

> NOTE TO CLAUDE CODE: leave clearly marked placeholder text (e.g. `[ADD PROJECT NAME]`, `[ADD SCREENSHOT]`, `[ADD LIVE LINK]`) for any section not filled in above, so it's obvious what still needs to be completed before deploying.

### 3. "How I work" section
Short section, 3-4 bullet points, scannable:
- Fixed-price and timeline-based engagement options
- Direct communication — fast turnaround, English-fluent, works async-friendly with US time zones
- AI-assisted development workflow — used deliberately to ship faster without sacrificing code quality (frame as a strength, not a gimmick)
- Full-stack ownership — architecture through deployment (auth, billing, CI/CD), not just frontend/backend pieces

### 4. Social proof section
- Placeholder for 1-3 testimonials, structured as quote + name + role/company
- Since none exist yet, use a subtle placeholder block: `[Testimonials will go here — leave section commented out or hidden until first client testimonials are available]`

### 5. Final CTA section
- Repeat the primary call to action clearly: one button, "Book a call" or "Message me"
- Short supporting line: e.g. "Currently taking on 1-2 new projects — let's talk about what you're building."

## Footer
- Simple: name, email/contact link, GitHub link, LinkedIn/X link (placeholders where needed)

## What NOT to do
- No stock photos of generic "business people shaking hands"
- No walls of paragraph text — bullet points and short lines only
- No more than one CTA style/color so it doesn't compete with itself
- Don't invent fake metrics, fake user counts, or fake testimonials — leave those sections as clearly marked placeholders until real data exists

## Deliverable
A single deploy-ready page (e.g. `index.html` + `style.css`, or equivalent single-page app structure) in this folder, with clearly marked placeholders for anything not yet filled in (project 2/3/4 details, live links, screenshots, testimonials, contact links).
