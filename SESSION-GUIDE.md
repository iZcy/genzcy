# Session Guide — Key Points Per Session

---

## Session 1 — "Introduction to Vibe Coding Responsibly"

**Goal:** Owner understands the landscape, the history, and ships their first (vanilla) site.

| Phase | Key points to present |
|---|---|
| **Compare paths** | Campus (+: research-ready, -: bad innovation, no skill). Practicals (+: superpower of creating everything, -: business-ignorant, best-case focus). Vibe Coder (+: fast-paced, innovators, closest to businesses, -: no fundamental, overconfident). Honest limitations of vibe coding. |
| **Dev history → Vibe Coding** | From punch cards → typed code → frameworks → AI. OpenCode + PromptAudit integration. How every prompt is logged. Explore OpenCode features. |
| **Zero-level stack** | Vanilla HTML/CSS/JS (no frameworks). Vanilla JS backend (no Express). SQLite (no MongoDB). Learn fundamentals BEFORE abstractions. |
| **Deploy** | Push to GitHub → Netlify auto-deploys. Manual connect: GitHub repo → Netlify. See it live. |

**Key outcomes:**
- Understands why this program exists (your honest take on all 3 paths)
- Sees OpenCode + PromptAudit working
- Ships a vanilla full-stack app to Netlify
- Knows the zero-level fundamentals before frameworks

---

## Session 2 — "The Prompt Architect"

**Goal:** Owner thinks like an architect. Context, SDLC, clean code, multi-project deployment.

| Phase | Key points to present |
|---|---|
| **AI history** | Expert systems (rules-based) → Statistical ML → LLMs (probabilistic). Why understanding this matters for prompting. |
| **Context management** | Markdowns for instructions. MCPs for tool access. Skills/Agents for specialized modes. Context window limits. |
| **SDLC + Blackbox Dev** | Liken to ML training loop: prompt (input) → test (evaluate) → error (loss) → adjust (retrain). Error-driven development + Test-driven development. |
| **Clean code, clean repo** | AI generates debris (duplicate files, unused imports, dead code). Teach cleanup discipline. Dedup patterns. |
| **Fork → 2 projects** | Fork the repo. Maintain 2 projects from one context. Deploy both via push MCP → Netlify auto-updates. |

**Key outcomes:**
- Understands why LLMs work the way they do
- Manages context windows effectively (MCPs, skills)
- Applies SDLC via error-driven + test-driven loop
- Cleans up AI debris
- Runs 2 deployed projects from one codebase fork

---

## Session 3 — "Do Not Reinvent The Wheels"

**Goal:** Owner understands why frameworks exist, picks a stack, and ships a framework-based app.

| Phase | Key points to present |
|---|---|
| **Why frameworks?** | History of web dev: vanilla → jQuery → React/Vue. Tradeoffs: speed vs structure, flexibility vs convention. Why so many? Different problems need different tools. |
| **Our stack** | Vite + TailwindCSS (FE). Express JS (BE). MongoDB (DB). Why these: ecosystem, simplicity, production-ready. |
| **Complete beginner track** | Model data (Mongoose). CRUD API (Express routes). Dynamic UI (Vite + Tailwind). Connect FE to BE. |
| **Deploy framework app** | Build + deploy second app with the full stack. Compare to Session 1's vanilla version. |

**Key outcomes:**
- Can explain why frameworks exist (not just "because everyone uses them")
- Ships a Vite+Tailwind+Express+MongoDB app
- Understands the difference from vanilla (Session 1)
- Can describe their stack choices to others

---

## Session 4 — "Trust, But Verify"

**Goal:** Owner implements logging + analytics. Can trace errors AND business events.

| Phase | Key points to present |
|---|---|
| **Structured logging** | Replace console.log with pino. Every request, DB query, error is JSON. Log levels: info, warn, error. |
| **Break case** | Deliberately introduce a bug (missing API key, wrong collection name). Owner traces it via logs. Fixes it. |
| **Analytics** | Install Plausible/GA. Track: page views, form submissions, bookings, errors. |
| **Business case** | Simulate a visitor flow (Playwright/browser MCP). Watch analytics capture it in real-time. |
| **Dashboard** | Build a log viewer + analytics summary in admin area. Dev logs + business data in one place. |

**Key outcomes:**
- Reads pino logs to debug production
- Sets up analytics and reads the dashboard
- Can answer: "what happened?" (logs) + "what are customers doing?" (analytics)
- Has a traceability system for future sessions

---

## Session 5 — "From Click to Cash"

**Goal:** Booking + payment flow end-to-end. Revenue goes through the site.

| Phase | Key points to present |
|---|---|
| **Booking flow** | Form (service + date + time + customer info) → availability check → confirmation. |
| **Payment** | Midtrans/Stripe/Xendit integration. Test mode. Never handle card data directly. |
| **Webhook** | Payment sends confirmation back to your server. Booking status updates. Email receipt via Resend. |
| **Break case** | Webhook not received → booking unpaid but created. Owner traces via logs, fixes webhook handler. |
| **Analytics event** | Track "booking_completed" as a conversion event. |

**Key outcomes:**
- Booking + payment works end-to-end in test mode
- Can debug webhook failures via logs
- Understands they never store card data
- Sees conversion event in analytics

---

## Session 6 — "Know Thy Customer"

**Goal:** Customer accounts, admin dashboard, role-based access.

| Phase | Key points to present |
|---|---|
| **Auth** | JWT tokens. Registration + login. Password hashing. Token stored in browser. |
| **Admin dashboard** | View all bookings, customers, services. Edit/delete. Status management. |
| **Roles** | Admin = everything. Customer = only their own bookings. Protected routes. |
| **Notifications** | Email (Resend) on booking status change. |
| **Break case** | Role leak — customer sees another customer's booking. Owner traces via auth logs, fixes role middleware. |
| **Analytics event** | Track "user_login", "booking_status_change". |

**Key outcomes:**
- JWT auth working with roles
- Admin dashboard with real management capabilities
- Can debug auth errors (401/403) via logs
- Understands role-based access control

---

## Session 7 — "Ready, Set, Ship"

**Goal:** SEO, performance, security, compliance. Site is production-ready.

| Phase | Key points to present |
|---|---|
| **SEO** | Meta tags, Open Graph, sitemap.xml, Google Search Console. |
| **Performance** | Image optimization, lazy loading, CDN, Lighthouse audit. |
| **Security** | Rate limiting, input validation, CORS, HTTPS enforcement. Cookie consent banner. Privacy page. |
| **Break case** | Mixed content warning (HTTP asset on HTTPS page). Owner traces via browser console, fixes to HTTPS. |
| **Analytics event** | Track Lighthouse score over time. |

**Key outcomes:**
- Site passes Lighthouse audit
- HTTPS enforced, no mixed content
- Cookie consent + privacy page live
- SEO meta tags + Open Graph working
- Can debug mixed content and CORS errors

---

## Session 8 — "Full Circle"

**Goal:** Solo build. Review growth. Community entry. Handoff.

| Phase | Key points to present |
|---|---|
| **Free build (60min)** | Owner builds ANYTHING they want. Mentor watches silently. They prompt, read, test, fix, deploy alone. |
| **PromptAudit review** | Review log across all 8 sessions. See prompt quality improve. Before/after comparison. |
| **Community showcase** | Present site to group. Answer questions. Other owners give feedback. |
| **Handoff conversation** | When to escalate to mentor. Pricing. Managed IT options. Goal #3 activated. |

**Key outcomes:**
- Solo feature built and deployed independently
- PromptAudit log shows measurable growth
- Joined the owner network
- Clear escalation path for when they scale

---

## Session Rhythm (120 min, every session)

```
00-05  Check-in, review PromptAudit feedback from last session
05-15  Concept — business analogy for today's topic
15-55  BUILD — owner prompts, AI builds, code appears
55-85  READ — owner reads every changed file, asks "what does this do?"
85-100 Error — break case or real error, trace and fix together
100-110 Commit + push (owner runs git commands)
110-120 Preview next session, update Build Journal
```
