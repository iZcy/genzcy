# Build With Vibe — Full Curriculum

> 4-week intensive 1-on-1 program. Business owners learn to architect, build, and ship their own website using AI-assisted development.

---

## Table of Contents

1. [Program Philosophy & the 3 Goals](#1-program-philosophy--the-3-goals)
2. [The Full-Stack Map](#2-the-full-stack-map)
3. [Phase 0 — Onboarding Audit](#3-phase-0--onboarding-audit)
4. [The 12 Architectural Concepts](#4-the-12-architectural-concepts)
5. [PromptAudit — The Two Sides](#5-promoptaudit--the-two-sides)
6. [Week 1 — Internet + Development](#6-week-1--internet--development)
7. [Week 2 — Frontend](#7-week-2--frontend)
8. [Week 3 — Backend + Database + APIs](#8-week-3--backend--database--apis)
9. [Week 4 — Deploy + Security + Analytics + AI](#9-week-4--deploy--security--analytics--ai)
10. [The 5-Layer Diagnostic Flow](#10-the-5-layer-diagnostic-flow)
11. [Owner's Technical Toolkit](#11-owners-technical-toolkit)
12. [Community Playbook](#12-community-playbook)
13. [Scale Handoff Script](#13-scale-handoff-script)
14. [Blank Vertical Sleeve Template](#14-blank-vertical-sleeve-template)
15. [Weekly Retrospective Format](#15-weekly-retrospective-format)

---

## 1. Program Philosophy & the 3 Goals

### Philosophy

Traditional programming education teaches you to **write code**. This program teaches you to **architect systems** and **direct AI to build them**. You won't become a developer — you'll become something more valuable: an architect who can commission, verify, and maintain software.

The curriculum is grounded in five principles (adapted from national curriculum standards):

| Principle | Meaning |
|---|---|
| **Learner-centered** | Every concept maps to YOUR business, not abstract exercises |
| **Contextual** | The vertical sleeve (your industry) shapes every example |
| **Essential** | Only concepts that improve prompt quality and architectural thinking |
| **Stakeholder-involved** | Mentor + owner + (eventually) their team collaborate |
| **Data-driven** | Weekly retrospectives use PromptAudit data + live analytics |

### The 3 Goals

**Goal #1 — Community.** Every graduate joins a network of business-owner builders. Shared vocabulary = shared identity = natural referrals and collaboration.

**Goal #2 — Common knowledge.** After 4 weeks, you speak the full-stack map fluently. Every future conversation about your website — with developers, designers, or vendors — becomes faster, clearer, and cheaper.

**Goal #3 — Scale.** When your business grows beyond what vibe coding can handle, you already have a trusted partner who understands your architecture. The curriculum is designed so that growth naturally returns to the mentor for managed IT services.

---

## 2. The Full-Stack Map

This is your new shared vocabulary. Every layer maps to something in your business.

```
Internet        Your shop front on the web
  Domain        Your address (yourbusiness.com)
  DNS           The phonebook that finds your address
  Hosting       The building where your shop lives
  HTTPS         The locked door

Frontend        What customers see and touch
  HTML          The structure (walls, rooms, signs)
  CSS           The paint, fonts, and decor
  JavaScript    The interactivity (doors that open, forms that submit)

Backend         What happens behind the counter
  Server        The kitchen that processes orders
  Business Logic  The recipes and rules
  Authentication  Who gets in (staff vs customers)

Database        Your filing cabinet
  Tables        The drawers (Customers, Orders, Products)
  Records       Each piece of paper in a drawer
  Relationships How drawers reference each other (this order belongs to that customer)

Integration     Connecting to the outside world
  APIs          Standard ways to talk to WhatsApp, payments, maps, etc.

Development     The tools you use to build
  Git           The save/undo/version system
  GitHub        The cloud backup + collaboration
  Local Environment  Your own computer's workshop

Deployment      Opening the shop to the public
  Build         Packing everything for shipping
  Hosting       Where the packed site lives
  CI/CD         Automatic quality checks + shipping

Security        Keeping things safe
  Passwords     The keys
  Permissions   Who can enter which rooms
  Secrets       API keys, database URLs — the master keys

Analytics       Understanding your customers
  Visitors      How many walked in
  Leads         How many filled out a form / called
  Conversions   How many bought / booked

AI Development  Your new superpower
  Prompting     Describing what you want in plain language
  Context       Giving the AI the information it needs (schema, style, constraints)
  Vibe Coding   The flow state of describing + building iteratively
```

**How to use this map:** When you write a prompt, mentally trace which layers it touches. "Add a booking form" = Frontend (form UI) + Integration (WhatsApp API) + Database (store bookings) + Security (owner-only access).

---

## 3. Phase 0 — Onboarding Audit

**When:** Session 0, 60-90 min before Week 1.
**Purpose:** Mirror's the curriculum development principle of "analyze characteristics" — every owner is different.

### Audit Questionnaire

| Area | Questions | Outcome |
|---|---|---|
| **Business** | What do you sell? Who buys it? What must the site achieve? | Owner's VMG (Vision/Mission/Goals for the site) |
| **Industry vertical** | Lead-gen / e-com / booking / portfolio / community / content? | Sleeve selection |
| **Existing assets** | Domain? Branding (logo, colors, fonts)? Content (copy, photos)? | Asset checklist |
| **Tech comfort** | Used a terminal? Git? Built anything before? Used AI coding tools? | Pacing calibration (beginner / intermediate) |
| **Integrations wanted** | Payments (Midtrans/Stripe)? WhatsApp? Google Calendar/Calendly? Maps? CRM? | Week 3 integration pick |
| **KPIs** | What does success look like in 30/60/90 days? | Analytics targets |
| **Scale intent** | Plan to grow? Hire a team? Add branches/services? Franchise? | Goal #3 handoff plan |
| **Prompting experience** | Used ChatGPT/Claude before? For what? How comfortable? | Baseline for PromptAudit |

### Output: Owner's Build Journal

A living document with these sections:
```
Owner Name:
Business:
Vertical Sleeve:
VMG:
Start Date:
Target KPIs:
PromptAudit Session Link:

Week 1 Goal:
Week 2 Goal:
Week 3 Goal:
Week 4 Goal:

Notes & Adjustments:
```

---

## 4. The 12 Architectural Concepts

These are the **mental models** you need to write high-quality prompts. Derived from analyzing 5 major developer curricula (The Odin Project, FreeCodeCamp, App Academy, Full Stack Open, roadmap.sh) — filtered to only what a business owner needs.

| # | Concept | Why It Matters for Prompting | Week |
|---|---|---|---|
| 1 | **Client-Server Architecture** | Know what lives where. "This form validates on frontend, submits to backend." | W1 |
| 2 | **HTTP & Request Lifecycle** | URL → DNS → server → response. Debug "why is this page blank?" | W1 |
| 3 | **Frontend vs Backend** | Specify WHICH side a feature belongs to in your prompts | W2/W3 |
| 4 | **Data Modeling (Entities & Relationships)** | THE most important skill. "A User has many Orders, an Order has many Products" → AI builds the right schema | W3 |
| 5 | **CRUD Operations** | 90% of features = Create, Read, Update, Delete. Frame requests in these terms | W3 |
| 6 | **API (REST)** | How frontend talks to backend. "GET /orders returns order history" | W3 |
| 7 | **Authentication & Authorization** | "Users log in with Google" vs "Admins can delete" = different architecture | W3 |
| 8 | **State Management** | "After saving, update the list without refresh" requires state-awareness | W2/W3 |
| 9 | **Error Handling & Validation** | "What if email is invalid?" + "What if DB is down?" = robust prompts | W1-W4 |
| 10 | **Environment & Secrets** | API keys / DB URLs belong in `.env`, not code. Essential security concept | W3/W4 |
| 11 | **Deployment Environments** | local vs staging vs production. "Don't break my live site" | W4 |
| 12 | **Monitoring & Observability** | Logs, metrics, alerts. Know when something's wrong and describe it | W4 |

---

## 5. PromptAudit — The Two Sides

PromptAudit is the feedback loop that makes this program different. It has two sides:

### Side A: Your Proxy (Mentor's Infrastructure)

Every prompt you type and every AI response you receive is logged via our PromptAudit proxy. This allows your mentor to:
- See EXACTLY what you asked
- See EXACTLY what the AI returned
- Rate the quality of both your prompt and the AI's output
- Give you targeted feedback to improve your prompting

Your proxy is already configured. You don't need to set up anything.

### Side B: Git Commits (Your Side)

Every prompt produces a code change, and every code change is committed to git and pushed to GitHub. This creates a permanent version history:

```
Prompt 1: "Add booking form with date picker"
  → Commit: "feat: add booking form with date validation"

Prompt 2: "Connect form to WhatsApp API"
  → Commit: "feat: integrate WhatsApp booking notifications"

Prompt 3: "Style mobile-first"
  → Commit: "style: responsive booking form"
```

Your mentor can review the git log to see how your project evolved, and correlate commits with PromptAudit logs to give you feedback on the relationship between your prompts and the actual output.

### Consent & Privacy

- PromptAudit only logs when you opt in (per session)
- You can pause or revoke logging at any time
- Past data stays; no new data is logged after revocation
- Data auto-deletes after 30 days (configurable)
- You can download your own data at any time

---

## 6. Week 1 — Internet + Development

**Goal:** Understand the full-stack map, set up your development environment, and make your first git commit.

### Thread Structure

Each week has 4 threads woven together:

- **A — Concept:** What this layer is, analogies to your business
- **B — SEE:** Inspect the real system (DevTools, terminal, logs)
- **C — BUILD:** Vibe-code your actual site using AI + git
- **X — Error Logging:** Cross-cutting skill that deepens each week

### Session 1.1 — The Full-Stack Map + Client-Server

| Thread | Activity |
|---|---|
| **A. Concept** | Walk through the full-stack map. Every layer mapped to a business analogy. |
| **B. SEE** | Visit any live site (yours or a competitor's). Open DevTools → Network tab. Watch the request waterfall: DNS → TCP → TLS → Request → Response. |
| **C. BUILD** | Create your GitHub account. Mentor creates a private repo for your project. |
| **X. Error** | Terminal basics: what "command not found" means, what exit codes look like. |

### Session 1.2 — Local Dev Environment

| Thread | Activity |
|---|---|
| **A. Concept** | Your computer as a workshop. Local vs production environments. |
| **B. SEE** | Install VS Code, Node.js (latest LTS), Git. See each tool's version output. |
| **C. BUILD** | Run `npm create` to scaffold your project. Open in VS Code. See the file tree. |
| **X. Error** | "npm install" fails — read the error, identify the problem, fix it. First taste of debugging. |

### Session 1.3 — Domain, DNS, Hosting, HTTPS

| Thread | Activity |
|---|---|
| **A. Concept** | Domain = your address. DNS = phonebook. Hosting = the building. HTTPS = locked door. |
| **B. SEE** | Run `dig yourdomain.com` and `nslookup`. See the DNS records. Inspect SSL certificate in the browser. |
| **C. BUILD** | If owner doesn't have a domain, buy one together. Point DNS to a placeholder. |
| **X. Error** | What happens when DNS doesn't resolve? What an SSL error looks like in browser. |

### Session 1.4 — Git + GitHub + PromptAudit Setup

| Thread | Activity |
|---|---|
| **A. Concept** | Git = save points + undo. GitHub = cloud backup + mentor review. |
| **B. SEE** | Clone your repo. Inspect `.git` folder. Run `git log` to see the commit history (even if just initial commit). |
| **C. BUILD** | First vibe-coding task: "Create a simple homepage with your business name and tagline." Watch OpenCode build it, then auto-commit + push. |
| **X. Error** | Merge conflict — what it looks like, what causes it, how to resolve (with AI help). |

### Week 1 Retrospective

- [ ] Can you draw the full-stack map from memory?
- [ ] Can you explain client-server to someone else?
- [ ] Can you open DevTools → Network tab and explain what you see?
- [ ] Can you run `git add`, `git commit`, `git push`?
- [ ] Did every prompt get committed and pushed to GitHub?
- [ ] PromptAudit check: mentor reviews 3 random prompts from the week

---

## 7. Week 2 — Frontend

**Goal:** Understand what the user sees and interacts with. Learn to inspect any website's structure and build your own.

### Session 2.1 — HTML: Structure

| Thread | Activity |
|---|---|
| **A. Concept** | HTML = the bones of your site. Heading, paragraph, list, link, image, form. |
| **B. SEE** | Open ANY site in DevTools → Elements tab. Inspect the DOM tree. Edit text live. Delete an element live (it comes back on refresh). |
| **C. BUILD** | Prompt: "Build the header and hero section of my site. My business is [name], my tagline is [tagline]." |
| **X. Error** | DevTools Console: see HTML parsing errors. Missing closing tag warnings. |

### Session 2.2 — CSS: Style

| Thread | Activity |
|---|---|
| **A. Concept** | CSS = the paint, fonts, spacing, layout. Same HTML, completely different look. |
| **B. SEE** | In DevTools, change colors, fonts, margins live. See the CSS box model on any element. |
| **C. BUILD** | Prompt: "Style my header with my brand colors (#hex1 and #hex2), make the nav horizontal, add hover effects." |
| **X. Error** | CSS not applying — specificity issues, missing semicolon, wrong selector in DevTools. |

### Session 2.3 — JavaScript: Behavior

| Thread | Activity |
|---|---|
| **A. Concept** | JS = interactivity. Forms that validate, buttons that do things, data that updates without refresh. |
| **B. SEE** | See Console tab in action. Run a simple JS command live on any page. See errors with line numbers. |
| **C. BUILD** | Prompt: "Add a mobile hamburger menu to my nav that shows/hides on click. Add a smooth scroll to sections." |
| **X. Error** | Console errors: `Uncaught TypeError`, `is not defined`, `null is not an object`. Read the line number, inspect the source. |

### Session 2.4 — Components + DevTools Deep Dive

| Thread | Activity |
|---|---|
| **A. Concept** | Components = reusable building blocks. Same card component, different data. |
| **B. SEE** | Deep DevTools: Network tab (file sizes, load times, 404s), Application tab (cookies, localStorage), Lighthouse audit. |
| **C. BUILD** | Prompt: "Create a pricing card component with 3 tiers. Each card has name, price, features list, and a CTA button. Use my brand colors." |
| **X. Error** | Network tab hunt: find a 404, a slow-loading image, a script that failed. Fix them. |

### Week 2 Retrospective

- [ ] Can you inspect any website's HTML and CSS in DevTools?
- [ ] Can you identify JavaScript errors in the Console?
- [ ] Can you check what files are loading (or failing) in the Network tab?
- [ ] Is your site's frontend built and styled?
- [ ] PromptAudit check: mentor reviews prompt quality for specificity (did they mention colors, layout, mobile?)

---

## 8. Week 3 — Backend + Database + APIs

**Goal:** Understand what happens behind the scenes. Model your business data. Connect real integrations.

### Session 3.1 — Server + Request Lifecycle

| Thread | Activity |
|---|---|
| **A. Concept** | Server = the kitchen. Request comes in, order is processed, response goes out. Business logic = the recipes. |
| **B. SEE** | See the server console log output. Start/stop the dev server. See each request logged with method, path, status code. |
| **C. BUILD** | Prompt: "Create a simple API endpoint that returns my business info as JSON: name, address, phone, hours." Then visit it in browser. |
| **X. Error** | Server crash — read the stack trace. Identify the file and line number. See what was passed vs expected. |

### Session 3.2 — Database: Tables, Records, Relationships

| Thread | Activity |
|---|---|
| **A. Concept** | Database = your filing cabinet. Tables = drawers. Records = papers. Relationships = references between drawers. |
| **B. SEE** | Open a database browser (TablePlus / Prisma Studio). SEE your actual tables. SEE the rows. Run a `SELECT` query. |
| **C. BUILD** | Prompt: "Create a database model for my business: [describe entities]. A Customer has many Bookings. A Booking belongs to one Service." |
| **X. Error** | DB connection refused — what it means (wrong host/port/credentials). Query error — syntax or missing table. |

### Session 3.3 — Authentication

| Thread | Activity |
|---|---|
| **A. Concept** | Auth = who are you? (login) + what can you do? (permissions). Passwords, tokens, sessions. |
| **B. SEE** | Inspect the login flow. See the token in Application tab (cookies/localStorage). See the `.env` file where secrets live. |
| **C. BUILD** | Prompt: "Add login with email and password. Only authenticated users can create bookings. Admin can view all bookings." |
| **X. Error** | Login fails — inspect the Network tab: was the request sent? What status code? What error message? |

### Session 3.4 — APIs: Real Integration

| Thread | Activity |
|---|---|
| **A. Concept** | API = a contract. Your site talks to WhatsApp / payments / maps through a defined interface. |
| **B. SEE** | In DevTools Network tab, filter to XHR/Fetch. See the raw API request (headers, body) and response (data, status). |
| **C. BUILD** | Prompt: "Connect my booking form to WhatsApp. When someone submits, send a WhatsApp message to me with their name, phone, and preferred date." |
| **X. Error** | API returns 400/401/403/500 — what each means. API key invalid — check `.env`. Rate limit — wait or upgrade. |

### Week 3 Retrospective

- [ ] Can you open the database and see your data?
- [ ] Can you trace a request from button click → API call → server → database → response?
- [ ] Can you read a server error stack trace?
- [ ] Are your integrations working?
- [ ] PromptAudit check: mentor reviews data modeling prompts — did they specify entities and relationships?

---

## 9. Week 4 — Deploy + Security + Analytics + AI

**Goal:** Ship your site to the real internet, secure it, measure it, and learn to continue building independently.

### Session 4.1 — Build & Deploy

| Thread | Activity |
|---|---|
| **A. Concept** | Deploy = moving from your workshop (localhost) to the storefront (production). Build = packing everything efficiently. |
| **B. SEE** | See the build output (bundled files). See the production logs. Compare dev vs prod environments. |
| **C. BUILD** | Deploy to production. Set up a custom domain. Enable HTTPS. |
| **X. Error** | Production error — check logs, is it the same as local? Configuration difference? Rollback strategy. |

### Session 4.2 — Security

| Thread | Activity |
|---|---|
| **A. Concept** | Security = who gets in, what they can do, what secrets are exposed. |
| **B. SEE** | Audit `.env` — are all secrets there? Browser Application tab — what's exposed in cookies/storage? Network tab — are API keys visible? |
| **C. BUILD** | Prompt: "Move all secrets to environment variables. Ensure no API keys are in client-side code. Add rate limiting to the booking endpoint." |
| **X. Error** | Security scan: try to access something you shouldn't. What does a 403 look like? What does an exposed .env look like? |

### Session 4.3 — Analytics

| Thread | Activity |
|---|---|
| **A. Concept** | Analytics = knowing your customers. Visitors → Leads → Conversions. Without data, you're guessing. |
| **B. SEE** | Install Plausible or Google Analytics. See the live dashboard. Watch your first real visitor appear. |
| **C. BUILD** | Prompt: "Track form submissions as conversion events. Show a simple dashboard in my admin area with visitor count and conversion rate." |
| **X. Error** | Analytics not tracking — check the Network tab for the analytics script. Is it loading? Is there a content blocker? |

### Session 4.4 — AI Independence

| Thread | Activity |
|---|---|
| **A. Concept** | AI = your junior developer. You describe, it builds, you verify. The more context you give, the better it performs. |
| **B. SEE** | Review your own PromptAudit log from the past 3 weeks. See how your prompts improved. Identify patterns. |
| **C. BUILD** | Solo challenge: "Add a new page to my site with [feature]. I'll write all the prompts myself." Mentor observes silently. |
| **X. Error** | AI hallucination — the AI generated something that doesn't exist. How did you catch it? What did you learn? |

### Session 4.5 — Community Handoff + Scale

| Thread | Activity |
|---|---|
| **A. Concept** | You're now a member of a network. Other owners need what you just learned. When you scale, you'll need expert help. |
| **B. SEE** | Tour the community: see other owners' sites, see what's possible in later stages. |
| **C. BUILD** | Your site is live. Your analytics are running. Your PromptAudit log shows 15+ prompt cycles. You're ready. |
| **X. Error** | Final review: what happens if your site goes down? Who do you call? What information do you need to provide? (This IS the handoff conversation.) |

### Week 4 Retrospective

- [ ] Is your site live on your own domain with HTTPS?
- [ ] Can you check production logs?
- [ ] Can you read your analytics dashboard and identify trends?
- [ ] Can you independently prompt AI to add a new feature?
- [ ] Do you know what information to give a developer when something breaks?
- [ ] Have you been introduced to the community?

---

## 10. The 5-Layer Diagnostic Flow

When something breaks, follow this checklist. It traces the problem from the user's screen to the database.

```
Layer 1: USER REPORT
  "The booking form isn't working."
  ↓

Layer 2: BROWSER CONSOLE (DevTools)
  Open Console tab → any red errors?
  Open Network tab → find the failed request
  What status code? 404 (not found) / 500 (server error) / 4xx (client error)
  ↓

Layer 3: SERVER LOGS
  Check the server console / log file
  Find the request that matches the Network tab failure
  Read the stack trace — what file, what line, what was passed?
  ↓

Layer 4: DATABASE
  Open the database browser
  Does the relevant table exist? Does it have the expected columns?
  Is the data there? Try a manual query.
  ↓

Layer 5: EXTERNAL API / INTEGRATION
  Is the external service (WhatsApp, payment, etc.) working?
  Is the API key valid? Has it expired?
  Is there a rate limit or outage?
```

**Owner's rule:** By the time you call your mentor, you should be able to say: "The booking form returns a 500. The server log says the WhatsApp API returned a 401. I checked the `.env` and the API key looks correct. Can you help me check if the key expired?"

This level of description halves debugging time and makes the handoff (Goal #3) seamless.

---

## 11. Owner's Technical Toolkit

### Can DO

| Tool | What you can do independently |
|---|---|
| **VS Code** | Open files, edit text, run terminal, install extensions |
| **Terminal** | Run commands your mentor gives you, start/stop dev server, run git |
| **Git** | Add, commit, push, check status, view log |
| **GitHub** | Create repo, clone, push, view commits online, open PR |
| **OpenCode** | Start it, type prompts, see it build |
| **PromptAudit** | Toggle consent, review your own log |
| **Deploy** | Deploy via command, check if site is live |
| **Analytics** | View dashboard, understand visitors/leads/conversions |

### Can READ / DIAGNOSE

| Tool | What you can read and understand |
|---|---|
| **Browser DevTools** | Inspect DOM, edit CSS live, read Console errors, see Network waterfall, inspect cookies/storage |
| **Server logs** | Read stdout/stderr, identify file/line in stack trace, understand 4xx/5xx |
| **Database browser** | See tables, rows, relationships; run basic SELECT queries; spot nulls or missing data |
| **Git log** | Read commit history, understand what each change was |
| **Analytics dashboard** | Read visitor count, conversion funnel, event stream |
| **Error tracker (if configured)** | Read error report, identify frequency and affected users |
| **`.env` file** | Audit what secrets exist, check if anything is missing or duplicated |

---

## 12. Community Playbook

**Goal:** Every graduate joins an ongoing network, creating the "new way to network" (Goal #1).

### Onboarding

1. **Graduation showcase** — Each owner's live site is presented to the group. They explain what they built, how they built it, and what they'd do next.
2. **Community entry** — Owner is added to a private group (Telegram/Discord/Slack). They get a profile: name, business, site URL, vertical, PromptAudit session link.
3. **First connection** — Mentor introduces them to 2-3 other owners in related or complementary verticals.

### Ongoing

- **Monthly showcase** — Owners share new features they built independently
- **Vertical channels** — #fb-owners, #services, #ecom, etc. — shared templates, integrations, tips
- **Prompt swap** — Owners share effective prompts they discovered
- **Mentor AMA** — Monthly open Q&A session
- **Referral bounties** — When an owner refers someone new, they get credit toward managed IT services

### Network Effect (Goal #1 → Goal #3)

Owners refer each other for business. When an owner's business grows and they need more than vibe coding can provide (custom features, team access, multi-location, compliance), they naturally return to you. The community becomes your inbound sales channel.

---

## 13. Scale Handoff Script

The **trigger conversation** — when an owner's needs exceed what vibe coding can sustain, and they should return to you for managed IT services.

### Signs an Owner Should Hand Off

- "I need multiple people to manage the site"
- "I need custom features my devkit doesn't support"
- "I'm getting too many orders to manage manually"
- "I need to connect to enterprise systems (ERP, CRM)"
- "I need compliance (HIPAA, PCI, data protection)"
- "I want to franchise / open multiple locations"
- "I don't have time to maintain it myself"

### The Handoff Conversation

```
Owner: "I'm getting too many bookings to handle manually. I need an automated system."

You: "Great problem to have. Here's what I'd recommend:

Phase 1 (us): Full booking automation → integrated calendar → payment processing → $X/mo
Phase 2 (us): Customer portal → automated reminders → review system → $Y/mo
Phase 3 (us): Multi-staff management → analytics dashboard → $Z/mo

You focus on growing the business. I keep the tech running.

Because I already know your architecture (from the 4-week program), I can start immediately.
No discovery phase. No 'what does this code do?' Six weeks compressed to one."
```

### Pricing Framework (Your Side)

Offer a graduated path:
- **Retainer:** Monthly maintenance + uptime monitoring + minor updates
- **Project:** New features, integrations, scaling
- **Full managed:** Everything — owner never touches the code again

---

## 14. Blank Vertical Sleeve Template

Use this template when onboarding a new owner in an industry you haven't served before.

```
## [Vertical Name] Sleeve

### Owner Profile
- Typical business type:
- Typical owner comfort level:
- Typical budget range:

### Week 2 — Frontend Build
- What they build:
- UI components needed:
- Example prompt:

### Week 3 — Data Model
- Entities:
- Relationships:
- CRUD operations needed:

### Week 3 — Integration
- Primary integration:
- Secondary integration:
- API setup notes:

### Week 4 — KPIs
- Primary metric:
- Secondary metric:
- Analytics events:

### Week 4 — Scale Handoff
- Most likely scale trigger:
- Suggested handoff package:

### Notes
- Unique considerations:
- Common pitfalls:
- Good example sites:
```

---

## 15. Weekly Retrospective Format

Each week ends with a 30-minute retrospective between mentor and owner.

### Owner Self-Assessment (5 min)

Rate 1-5:
- I understand the concepts taught this week
- I can explain them to someone else
- I can use the tools independently
- My prompts are improving
- I feel confident about next week

### Mentor Assessment (10 min)

- Review PromptAudit log: 3 random prompts from the week
- Review git log: are commits descriptive? Is push working?
- Review live site (if applicable)
- Identify 1 thing to improve next week
- Identify 1 thing the owner excelled at

### Adjustments (10 min)

- Is pacing right? Speed up / slow down next week?
- Is the vertical sleeve working? Adjust examples?
- Any blockers (tools, understanding, motivation)?
- Update the Build Journal

### Preview (5 min)

- What's coming next week
- What to read/watch before the first session
- Any tools to install in advance

---

*This curriculum is a living document. Update it as you learn what works with each owner. The full-stack map stays the same; the sleeves evolve.*
