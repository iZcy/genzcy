# GenZCY — Private Class Flow

> End-to-end journey of the 1-on-1 mentorship program. Owner goes from zero to architect-literate in 4 weeks.

---

## Overview

```
Discovery ──> Phase 0 ──> 4-Week Program ──> Graduation ──> Scale
  |             |           |                    |              |
  v             v           v                    v              v
Intake      Onboard    8 sessions × 2h       Community      Managed IT
call        audit      = 16 hours            network        handoff
```

**Total owner time investment:** ~18 hours (1 onboarding + 16 sessions + 1 graduation showcase)

---

## Step 1: Discovery & Intake

**Format:** Free 30-min video call — owner decides if this is for them.

| What happens | Owner learns | I learn |
|---|---|---|
| I explain the program, the vibe-coding approach, and the 3 goals | What "vibe coding" means, that they won't learn to code but to architect | Their business type, their motivation, their budget |
| Owner describes their business and what they want to build | If this matches their expectations | Whether they're a good fit (motivated, willing to invest 4 weeks) |
| I show them the session table (the 11-column curriculum) | The full scope of the program | Their initial questions and concerns |
| I explain PromptAudit and OpenCode | How feedback and auditing works | Their tech comfort level |

**Outcome:** Owner either signs up (schedule Phase 0) or gets a referral to a simpler solution.

---

## Step 2: Phase 0 — Onboarding Audit (Session 0)

**Format:** 60-90 min dedicated session. Owner's Build Journal is created.

### The Audit

| Area | Questions I ask | What it produces |
|---|---|---|
| **Business** | What do you sell? Who buys? What must the site achieve? | Owner's VMG (Vision/Mission/Goals for the site) |
| **Industry vertical** | Lead-gen / e-com / booking / portfolio / community / content? | Sleeve selection (F&B, services, retail, clinic, creative) |
| **Existing assets** | Domain? Logo? Brand colors? Fonts? Photos? Copy? | Asset checklist — what's ready, what's needed |
| **Tech comfort** | Used a terminal? Git? Built anything? Used AI? | Pacing calibration: beginner / intermediate |
| **Integrations wanted** | Payments? WhatsApp? Google Calendar? Maps? CRM? | Week 3 integration pick |
| **KPIs** | What does success look like in 30/60/90 days? | Analytics targets for Week 4 |
| **Scale intent** | Plan to grow? Hire? Add branches? Franchise? | Goal #3 handoff plan |
| **Prompting experience** | Used ChatGPT/Claude? For what? How comfortable? | PromptAudit baseline |

### Output: Owner's Build Journal

```yaml
owner: Jane Doe
business: Jane's Pet Services
vertical: Professional Services (booking)
vmg: "Customers can see services, book appointments, and I get WhatsApp notifications"
start_date: 2026-06-22
target_kpis: 50 bookings/month within 60 days
promptaudit_link: <generated>
pacing: beginner (never used terminal or git)
integrations: WhatsApp + Google Calendar
scale_intent: 3 branches in 2 years → managed IT needed
```

### Owner prepares before Week 1

- [ ] Gather brand assets (logo, colors, 3-5 product/service photos)
- [ ] Write 3-5 sentences about each service they offer
- [ ] Create a list of 5-10 customer testimonials (if available)
- [ ] Think of 2 competitor websites they like (for style reference)
- [ ] Install VS Code (I walk them through it if needed)

---

## Step 3: The 4-Week Program (8 Sessions × 2h)

**Schedule:** Typically 2 sessions/week (e.g., Tuesday + Thursday). Each session follows the same rhythm.

### Session Rhythm (120 min)

```
[00-05]  Check-in: what happened since last session, any blockers
[05-10]  Concept intro: I explain the layer/concept using business analogy
[10-45]  SEE + BUILD: owner writes prompts, AI builds, I guide
[45-75]  Owner reads the generated code in VS Code, asks questions
[75-90]  Error logging: something breaks → we trace and fix together
[90-110] Owner continues building solo (I observe silently)
[110-115] Commit + push to GitHub
[115-120] Wrap-up: what we learned, what's next, preview next session
```

### Session Breakdown

| Ses | Title | Key moment |
|---|---|---|
| 1 | **How the Web Works** | First prompt → first site → first git push. The dopamine hit. |
| 2 | **Domain + Feedback** | Buy their domain. Turn on PromptAudit. They see their own prompt history. |
| 3 | **Brand + Layout** | Their site starts looking like a real business. This is when it "clicks." |
| 4 | **Interaction** | They add a working feature (slider, menu, form). They feel capable. |
| 5 | **Their Data** | They see their own business data in a database. The "aha" moment. |
| 6 | **Logins + Connections** | WhatsApp notification fires when they test a booking. They're thrilled. |
| 7 | **Go Live + Measure** | Their site is on the real internet. They see their first real visitor. |
| 8 | **Solo + Community** | They build solo while I watch. Then they join the network. Graduation. |

### During the Program, I do:

- Review every prompt via PromptAudit (between sessions, ~15 min/session)
- Give written feedback on 3 prompts per session: what worked, what to improve
- Track their pacing — slow down or speed up based on confidence
- Update their Build Journal after each session

---

## Step 4: Graduation & Community Entry

**Format:** 30-min showcase session (can be group session with other graduates).

### Graduation Requirements

- [ ] Live site on their own domain with HTTPS
- [ ] At least 1 integration working (WhatsApp / payment / booking / etc.)
- [ ] Analytics installed with KPIs defined
- [ ] 1 solo-built feature (no mentor help during the build)
- [ ] PromptAudit log shows 15+ prompt cycles with improving quality
- [ ] Can explain their own architecture (the full-stack map from their site)

### What they get

- **Community badge** — added to the GenZCY owner network (Telegram/Discord)
- **Graduation showcase** — their site presented to the group; they explain their journey
- **PromptAudit portfolio** — their prompt history is their credential
- **Referral program** — refer another owner → credit toward managed IT services

### Community Ongoing (Goal #1)

- Monthly showcase: owners share features they built independently
- Vertical channels: #fb-owners, #services, #ecom, #clinic, #creative
- Prompt swap: owners share effective prompts they discovered
- Mentor AMA: monthly open Q&A
- Referral bounties: refer a new owner → discount on managed IT

---

## Step 5: Scale Handoff (Goal #3)

**Trigger:** Owner needs a feature that's too complex for vibe coding, or their business is growing beyond what they can manage solo.

### When to escalate

| Trigger | Example | Handoff to me |
|---|---|---|
| Multi-user / team | "I need 5 staff accounts with different permissions" | Build team auth + roles |
| Complex automation | "When a booking is confirmed, also send an email and update my CRM" | Build workflow automation |
| High traffic | "My site is slow during lunch rush" | Infrastructure scaling |
| Compliance | "I need patient data to be HIPAA-compliant" | Security audit + compliance |
| Mobile app | "I want an app, not just a website" | Build mobile app |
| Custom feature | "I need a booking algorithm that optimizes staff schedules" | Custom development |

### Pricing Framework

```
Phase 1 (light):  Maintenance + uptime monitoring + minor updates → $X/mo
Phase 2 (growth): New features + integrations + automation → $Y/mo  
Phase 3 (full):   Everything managed — owner never touches the code → $Z/mo
```

Because I already know their architecture (from the 4-week program), I can start immediately — no discovery phase, no ramp-up.

---

## The Full Cycle

```
                    ┌────────────────────────────┐
                    │     DISCOVERY CALL          │
                    │   Owner decides to join     │
                    └────────────┬───────────────┘
                                 │
                    ┌────────────▼───────────────┐
                    │     PHASE 0 — ONBOARDING    │
                    │   Audit → Build Journal     │
                    └────────────┬───────────────┘
                                 │
                    ┌────────────▼───────────────┐
                    │     WEEK 1-4 PROGRAM        │
                    │   8 sessions × 2h           │
                    │   ┌───┐ ┌───┐ ┌───┐ ┌───┐  │
                    │   │ W1│ │ W2│ │ W3│ │ W4│  │
                    │   └───┘ └───┘ └───┘ └───┘  │
                    └────────────┬───────────────┘
                                 │
                    ┌────────────▼───────────────┐
                    │     GRADUATION              │
                    │   Showcase → Community      │
                    └────────────┬───────────────┘
                                 │
                    ┌────────────▼───────────────┐
                    │     ONGOING                 │
                    │   Owner builds solo         │
                    │   Community events          │
                    │   Referral bounties         │
                    └────────────┬───────────────┘
                                 │
                    ┌────────────▼───────────────┐
                    │     SCALE HANDOFF (Goal #3) │
                    │   Owner grows → calls me    │
                    │   Managed IT services       │
                    └────────────────────────────┘
```
