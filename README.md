# Build With Vibe — Website Context Kit

> A curriculum + toolchain for business owners who want to understand how websites work, build their own with AI assistance, and scale with confidence.

---

## How Programming Was

Before 2023, building a website meant writing every single line of code by hand. You learned HTML, CSS, JavaScript, a backend language, SQL, and deployment — each taking months to years. The process was **deterministic**: you wrote exact instructions (code), the computer executed them exactly as written. If it broke, you read the code, found the typo, fixed it, redeployed. Slow but predictable.

A simple booking form could take a professional developer 2-3 days. A full business site: weeks to months.

---

## How Vibe Coding Changed It

Today, you describe what you want in plain language — a **prompt** — and an AI model generates the code. This is "vibe coding": you stay in the flow, describe features conversationally, and the AI builds them. What took weeks now takes hours.

But there's a catch.

---

## How LLMs Actually Work (The Black Box)

LLMs (Large Language Models) are **probabilistic**, not deterministic. They don't "understand" code like a human does. They predict the most likely next word (or line of code) based on patterns in their training data.

**Key implications:**

- **Same prompt can give different results.** Run it twice, get two answers. One might work, one might not.
- **They sound confident even when wrong.** An LLM will generate code with a fake API, a made-up function name, or a security hole — and explain it with perfect grammar.
- **They have no memory of your full architecture.** Each response is generated fresh. The model doesn't know your database schema unless you explicitly tell it in the prompt.
- **They can't test their own output.** The AI generates code, but only YOU (or a running program) can verify it works.

This is why **testing and error logging are not optional** — they are the only way to tame the black box. Every AI-generated feature must be run, observed, and verified. Errors are not failures; they are the model telling you what it needs next.

---

## Our Assisted Development Workflow

```
[ You describe what to build ] ──→ [ AI generates code ]
                                          │
                                          ▼
                              [ Run + test + observe ]
                                          │
                                          ▼
                              [ Commit + push to GitHub ]
                                          │
                                          ▼
                              [ Mentor reviews + PromptAudit logs ]
```

### The 3 pillars:

**1. OpenCode** — You talk to an AI assistant that edits your project files directly. Your prompts become real code.

**2. Git + GitHub** — After every prompt, changes are automatically committed and pushed. This creates a full history of every change, which your mentor (and future you) can review.

**3. PromptAudit** — Your prompts and the AI's responses are logged via our proxy system. This lets your mentor see what you asked, what the AI returned, and give targeted feedback to make your prompts better over time.

---

## Quick Start

```bash
# 1. Clone this repo
git clone https://github.com/your-org/website-context-kit.git my-website

# 2. Enter the project
cd my-website

# 3. Install OpenCode (if not already installed)
npm install -g @opencode-ai/cli

# 4. Start building
opencode
```

OpenCode will read the `AGENTS.md` instructions and automatically commit + push after every task. You just describe what to build.

---

## What You'll Learn (4 Weeks)

| Week | Topic | You'll be able to... |
|---|---|---|
| 1 | How the web works + dev environment | Explain the full stack, use git, run a local server |
| 2 | Frontend | See any website's structure in DevTools, build your own UI |
| 3 | Backend + Database + APIs | Model your business data, connect real integrations |
| 4 | Deploy + Security + Analytics + AI | Ship live, monitor visitors, continue building with AI |

Full curriculum at `CURRICULUM.md`.

---

## The Full-Stack Map (Your New Vocabulary)

```
Internet        Domain · DNS · Hosting · HTTPS
Frontend        HTML · CSS · JavaScript
Backend         Server · Business Logic · Authentication
Database        Tables · Records · Relationships
Integration     APIs
Development     Git · GitHub · Local Environment
Deployment      Build · Hosting · CI/CD
Security        Passwords · Permissions · Secrets
Analytics       Visitors · Leads · Conversions
AI Development  Prompting · Context · Vibe Coding
```

Every layer has a purpose. After 4 weeks you'll know what each one does, how they connect, and when to ask for help (Goal #3).

---

## The 3 Goals

1. **Community** — You're not alone. Join a network of business owners who speak the same language and help each other grow.
2. **Common knowledge** — You understand the structure. This makes every future conversation about your website faster and clearer.
3. **Scale** — When you grow, you'll need expert help. You already know us, we already know your architecture. Easy.
