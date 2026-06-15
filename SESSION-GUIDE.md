# Session Guide — Key Points Per Session

---

## Session 1 — "My First Page" (Full Stack in One Page)

**Goal:** Owner builds first page + understands what FE/BE/DO are by DOING them.

| Key points to present | Owner should walk away knowing |
|---|---|
| **How development changed:** Old way = write every line by hand, deterministic, months to build. New way (vibe coding) = describe what you want in plain language, AI generates the code, hours to build. | AI is **probabilistic** — it predicts, doesn't "think." Same prompt can give different results. You MUST test everything and read the generated code. You don't learn to code; you learn to **architect and direct**. |
| Frontend = what users see (HTML/CSS) | They built HTML, saw it render in browser |
| Backend = server that delivers pages (Express) | They started a server, saw it respond to requests |
| DevOps = git + deploy + monitor (Git + GitHub) | They ran `git init`, committed, pushed to GitHub |
| PromptAudit protocol activated | Every prompt gets a before/after commit pair |
| Production tool: **Vite** scaffolds the project | They'll never write raw HTML files |

**The definition moment:** Owner sees their page in browser → "I made that."

---

## Session 2 — "Brand + Contact"

**Goal:** Site looks like their business. Customers can reach them.

| Key points to present | Owner should walk away knowing |
|---|---|
| CSS = brand identity (colors, fonts, layout) | Site now has their logo, brand colors, looks professional |
| Mobile-first = most visitors are on phones | Layout works on both phone and desktop |
| Form data goes to the server (Express POST) | They see form submission hit terminal + receive email |
| Production tool: **Resend** sends the email | One API key, no SMTP config |
| Branches = safe experiments (`git branch`) | They branched, made changes, merged back |
| `.gitignore` protects secrets | API keys don't go to GitHub |

**The click moment:** Owner submits form → gets email → "It actually works."

---

## Session 3 — "Content + SEO"

**Goal:** Google can find and understand the site.

| Key points to present | Owner should walk away knowing |
|---|---|
| SEO = how Google discovers your site | Meta tags, Open Graph, sitemap.xml |
| Google Search Console = monitor your presence | Submitted sitemap, verified ownership |
| Database = structured storage (MongoDB) | Collections = folders, documents = files |
| Production tool: **MongoDB + Mongoose** | Connected to MongoDB, created Service model |
| FAQ accordion = trust signal | Interactive content that answers customer questions |

**The discovery moment:** Owner sees their database with real data → "My business has a digital filing cabinet."

---

## Session 4 — "Live Data"

**Goal:** Site content comes from the database, not hardcoded.

| Key points to present | Owner should walk away knowing |
|---|---|
| Dynamic vs static content | Services page reads from DB, updates automatically |
| CRUD = Create, Read, Update, Delete | Admin page: add/edit/delete services |
| API = waiter between frontend and database | They see raw JSON responses in browser |
| Password protection = basic security | Admin area locked, security mindset begins |

**The aha moment:** Owner edits a service in admin → changes appear instantly on live page → "I just updated my site without touching code."

---

## Session 5 — "Bookings + Maps + Payments"

**Goal:** Customers can book, pay, and find the business location.

| Key points to present | Owner should walk away knowing |
|---|---|
| Booking form = date picker + time slot + service | Customer selects service, date, time, submits |
| Payment gateway = Midtrans/Xendit/Stripe | Test mode transaction flows end-to-end |
| Webhooks = payment sends confirmation back | Server receives webhook, updates booking status |
| Google Maps embed | Location shown on site, click for directions |
| Never log card details | Payment security awareness |

**The thrill moment:** Owner submits a test booking with payment → sees it in admin → gets webhook → "This is a real business tool."

---

## Session 6 — "Logins + Dashboard + Privacy"

**Goal:** Owner controls access. Customers have accounts. Privacy compliant.

| Key points to present | Owner should walk away knowing |
|---|---|
| Auth = who can do what | Login page, JWT token, role-based access |
| Dashboard = manage bookings + customers | Admin sees all, customer sees only theirs |
| Cookie consent = legal requirement | Banner appears, user choices respected |
| Secrets audit = full review | Every API key checked, rotated, .env verified |
| Production tool: **JWT** for auth tokens | Stateless, secure, industry standard |

**The control moment:** Owner logs in → sees dashboard with real data → "I can run my business from here."

---

## Session 7 — "Deploy + Analytics + Performance"

**Goal:** Site is live, secure, fast, and measurable.

| Key points to present | Owner should walk away knowing |
|---|---|
| 🔒 HTTPS = green lock in browser | SSL certificate installed, secure connection |
| Production ≠ development | Configs differ, errors happen differently |
| Analytics = know your customers (Plausible/GA) | First real visitor appears on dashboard |
| CDN = fast loading worldwide | Images served from edge, pages load faster |
| 404 page + loading states = professional UX | Broken links show helpful page, not errors |
| Rollback = safety net | If deploy breaks, revert to previous version |
| Production tool: **pino** for structured logs | Logs are JSON, readable, parseable |
| Production tool: **Nginx/Caddy** as reverse proxy | Handles SSL, static files, load balancing |

**The milestone moment:** Owner visits their site on their domain with HTTPS → analytics shows first visitor → "It's a real website now."

---

## Session 8 — "Solo + Community"

**Goal:** Owner builds a feature entirely alone. Graduates into the network.

| Key points to present | Owner should walk away knowing |
|---|---|
| **Solo challenge:** mentor watches silently | Owner writes all prompts, reads all code, fixes all errors |
| PromptAudit log review | See improvement across 7 sessions |
| Community entry | Other owners, vertical channels, monthly AMA |
| Scale handoff conversation | When to call for help, pricing, next steps |

**The graduation moment:** Owner presents their site to the group → other owners ask questions → they answer confidently → "I can do this."

---

## Session Rhythm (Fixed, Every Session)

| Time | Activity |
|---|---|
| 00-05 | Check-in, review PromptAudit feedback |
| 05-15 | Concept — business analogy for today's layer |
| 15-55 | BUILD — owner prompts, AI builds, code appears |
| 55-85 | READ — owner reads every changed file, asks "what does this do?" |
| 85-100 | Error — something breaks, trace and fix together |
| 100-110 | Commit + push (owner runs git commands) |
| 110-120 | Preview next session, update Build Journal |
