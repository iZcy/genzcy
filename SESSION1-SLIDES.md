# Session 1 — Google Slides Guide

---

## Slide 1 — Title Slide

**What to show:** Program title + your face/logo
**What to say:** "Welcome to Private Vibe Coding with Fundamentals Mentorship. I'm Yitzhak Edmund Tio Manalu."

---

## Slide 2 — Session Rhythm

**What to show:** A simple 6-step flow
```
Konsep → BUILD via Prompt → BACA Kode → Error → Commit & Push
```

**What to say:** "Every session follows this same rhythm. We learn a concept, build via AI, read what was generated, break something and fix it, then save and push. You'll get used to this flow by Session 3."

---

## Slide 3 — The 3 Paths (Your Hot Take)

**What to show:** A 3-column comparison table

| Campus | Proyek / Praktek | Vibe Coder |
|---|---|---|
| + Research ready | + Create everything | + Fast-paced |
| + Deep fundamentals | + Ship features | + Closest to business |
| - Bad innovation | - Business blind | - No fundamentals |
| - No practical skill | - Best-case focus only | - Overconfident |

**What to say:** "I've seen all three paths. Campus teaches you theory but you can't ship. Proyek teaches you to build but you miss the big picture. Vibe coding — what we're doing — gets you closest to your business, fastest. But you have to stay humble and keep learning fundamentals."

**Demo to show:** None — pure talk.

---

## Slide 4 — The Evolution of Development

**What to show:** A timeline graphic

```
Punch Cards → Terminal Code → Frameworks → AI Vibe Coding
(1960s)      (1980s)       (2000s)     (2023+)
```

**What to say:** "For 60 years, you had to write every character yourself. Now you describe what you want in plain language and AI builds it. You don't learn to code. You learn to architect and direct. That's what this program is about."

**Key point to emphasize:** "AI is probabilistic, not deterministic. It guesses the next word. Same prompt can give different results. You MUST test everything and read what AI produces."

---

## Slide 5 — Our Tools

**What to show:** 4 logos / icons
- VS Code
- OpenCode
- GitHub
- Netlify

**What to say:** "These 4 tools are all we need today. VS Code to edit files. OpenCode to talk to AI. GitHub to save and track changes. Netlify to put your site on the real internet."

**Demo to show:** Open VS Code. Open terminal. Type `code --version`, `node --version`, `git --version`.

---

## Slide 6 — OpenCode Tour

**What to show:** OpenCode interface (screenshot or live)
- Input prompt area
- File changes it makes
- Terminal output

**What to say:** "This is where you'll type your prompts. OpenCode reads your project files, understands the context, and makes edits. You describe what you want — it builds it."

**Demo to show:** Type a simple prompt: "Explain what files are in this project." Show the response.

---

## Slide 7 — PromptAudit (Your Side)

**What to show:** PromptAudit dashboard screenshot (your proxy interface)
- List of prompts
- AI responses
- Session timeline

**What to say:** "This is PromptAudit. Every prompt you type and every response AI gives is logged here. I review this between sessions to give you feedback on your prompting. It's how you get better. Only I see this — it's private between us."

**No demo needed** — just show the concept. They don't touch this.

---

## Slide 8 — Git & GitHub

**What to show:** A simple diagram
```
Local (your computer) → commit → GitHub (cloud) → deploy → Netlify (live)
```

**What to say:** "Git saves versions of your work. GitHub backs it up online. Netlify takes it from GitHub and puts it on the internet. Every time you push, Netlify auto-deploys."

**Demo to show:** 
- `git init`
- `git add -A`
- `git commit -m "first commit"`
- Go to GitHub, show the repo appeared
- "You run these commands. I'll guide you at first, but by Session 3 you'll do it automatically."

---

## Slide 9 — BUILD Time: Your First Page

**What to show:** A blank VS Code → result screenshot

**What to say:** "Now we build. Type this prompt into OpenCode — or say it in your own words."

**The prompt:**
> "Create a simple homepage for my business [their business name]. Include a hero section with the business name and tagline. Use vanilla HTML, CSS, and JavaScript. No frameworks."

**What they do:** Type the prompt. Watch OpenCode generate files.

**What you do after:** Open each file together. "This is HTML — it's the structure. This is CSS — it's the style. This is JS — it handles interactivity."

---

## Slide 10 — READ Phase

**What to show:** A screenshot of generated code with annotations
```
HTML: <h1>Business Name</h1>   →  The big heading
CSS:  .hero { background: ... } →  The colored section
JS:   console.log("hello")    →  A message in console
```

**What to say:** "Now we read what AI built. You don't need to memorize syntax. You need to understand the STRUCTURE. Open each file and follow along."

**What they do:** Click each file in VS Code. Read the code. Ask "what does this mean?"

**What you answer:** Plain language. "This line makes the heading big. This line sets the background color. This line runs when the page loads."

---

## Slide 11 — Error Time

**What to show:** A broken page screenshot (404 image, layout broken)

**What to say:** "Let's break something on purpose. I'll change a file name. Now open the site in browser — what happened?"

**The scenario:**
- Rename a CSS file or change an image path
- Show the 404 error in browser console
- "Read the error together. Can you tell what's wrong?"

**What they learn:** "Errors are not failures. They're instructions. The error tells you EXACTLY what's wrong. Read it."

---

## Slide 12 — Deploy to Netlify

**What to show:** Netlify dashboard steps
1. Log in to Netlify
2. Click "Add new site" → "Import from Git"
3. Select GitHub repo
4. Deploy

**What to say:** "This is the magic moment. We connect GitHub to Netlify, and your site goes live."

**What they do:** Watch the deploy. Get the live URL. Open it on their phone.

**What to say when the site loads:** "This is your website. On the real internet. Anyone can visit it. You built this in under 2 hours."

---

## Slide 13 — Recap & What's Next (if time allows)

**What to show:** A checklist

```
✅ Understand the 3 dev paths
✅ VS Code + OpenCode + Git installed
✅ First prompt typed
✅ First site built
✅ Error traced and fixed
✅ Pushed to GitHub
✅ Live on Netlify
```

**What to say:** "In one session, you went from zero to a live website. Next session: The Prompt Architect — we'll learn how to give AI better context, manage conversations, and keep your code clean."

**What to ask them:** "What feature do you want to add to your site? Think about it before next session."

---

## Summary Timeline for You

| Time | Slides | What you do |
|---|---|---|
| 00-05 | 1-2 | Welcome, explain rhythm |
| 05-15 | 3-4 | Campus vs Proyek vs Vibe Code. Dev evolution |
| 15-25 | 5-8 | Setup tools: VS Code, OpenCode, Git, PromptAudit tour |
| 25-45 | 9 | BUILD: First prompt, first page generated |
| 45-65 | 10 | READ: Open each file, explain structure |
| 65-80 | 11 | Error: Break something, trace, fix |
| 80-100 | 12 | Deploy to Netlify. See it live. |
| 100-120 | 13 | Recap, journal, preview S2 |
