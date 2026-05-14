# Build your life — An AI-Powered Life Tracker without the micromanaging

**A lightweight system that remembers your goals, learns how you operate, does the thinking for you every week, and doesn't breathe down your neck.**

---

## The problem with most life tracking tools

Most trackers fail for the same reason: **you do all the cognitive work.** You log, you interpret, you decide what it means, you figure out what to do next. After a few weeks, the friction wins. You stop.

The rest fail for the opposite reason: they're too heavy. The habit apps that turn your life into a game. The journaling systems that require a daily practice. They're all asking you to maintain a second job — managing the *system* itself.

And none of them remember you. Notion doesn't know your 5-year plan when you open Monday's task list. Habit trackers count streaks but have no idea why you started.

---

## What this system does differently

**This is a Cursor-native life operating system.** Your goals live in markdown files. An AI reads them every session — automatically. You never paste context. You never re-explain yourself.

But the more important thing isn't that it remembers your goals. It's that **it learns how you personally operate** — and adjusts accordingly.

### It adapts to your energy

When you report a high-energy week, the AI proposes bolder goals. When you report medium or low energy, it scales back without you having to say "go easy on me." If you activate crash mode (one word), all growth expectations pause for the week and the floor drops to the minimum. No guilt. No catch-up.

Over months, the system accumulates a picture of when you tend to crash, what drains you, and what consistently moves the needle — so proposals get more accurate over time.

### It knows your failure modes

During setup, you identify your **top 3 barriers** to actually sticking with a system like this. These get stored in your Life Arc. Every time you say "I'm stuck" or "I can't bring myself to [X]," the AI loads those barriers first and checks whether this is one of your known patterns — and if so, applies the counter-protocol *you* set for yourself during onboarding.

Not generic advice. Your patterns, reflected back at you.

### It builds a model of who you are

An optional 15-minute deep dive at the end of each weekly check-in accumulates over time into a profile — not a personality type, but a running record of what you've been drawn to, what you've been avoiding, and what that says about what you actually want. The AI uses this to push back with something like *"this is the third time this has come up around [X] — what do you think is driving it?"*

### The weekly check-in is 15 minutes. The AI does the rest.

Every week, you type `weekly check-in`. The AI:
- Loads your 1-year goals, last month's plan, and last 2 weeks of history — before you say a word
- Asks 7 rapid-fire questions (numbers and Y/N — no journaling required)
- Proposes 5 specific goals for the week based on your pace and what you've been avoiding
- Sets your 3 weekly reminders so you don't have to think about it during the week
- Flags if you're drifting off pace for the month — automatically

**You spend 15 minutes. The AI tracks the trend.**

### Monthly: you reflect, the AI synthesizes

Once a month, type `monthly reset`. The AI reads your full month of weekly data, runs 3 career clarity questions (your "Role Compass" — which builds signal over time on what kind of work actually fits you), and proposes next month's targets calibrated to your actual capacity, not an idealized version of yourself.

You confirm or adjust. One session. Everything is written.

### Yearly: the picture becomes clear

Quarterly reviews and a year-end synthesis reveal patterns you can't see week-to-week: how your energy correlates to your output, which pillars you systematically deprioritize, whether your stated career direction has been consistent or quietly shifting. The AI has kept every entry — nothing gets lost.

---

## The framework in 60 seconds

Your life has **pillars**: Career, Fitness, Social, Intellectual, Lifestyle. Each month, every pillar runs on one of four levels:

| Level | Effort | What it is |
|---|---|---|
| **Survive** | 3/10 — floor only | 3 fixed weekly habits; non-negotiable but minimal |
| **Sustain** | ~5/10 — acceptable | Last month's hardest thing, now being locked in |
| **Grow (primary)** | ~7/10 — uncomfortable | 1 main push this month |
| **Grow (secondary)** | ~5/10 | 1 push in a different pillar |

This means you are **never** being asked to grow in everything at once. The system respects that capacity is finite and that trying to improve everywhere simultaneously is how systems collapse.

**Rollover logic:** If you don't hit a grow target, it becomes next month's Sustain. Nothing is abandoned. Nothing is lost. The system accounts for real life.

**Crash mode:** Built-in. One word activates it. Expectations drop to any 2 of 3 survive goals for the week. No guilt architecture. No catch-up required.

---

## What makes this better than alternatives

| Tool | What it does well | What it misses |
|---|---|---|
| Notion / Obsidian | Flexible, pretty | You do all the thinking; no memory; no adaptation |
| Habit trackers (Streaks, Habitica) | Good for streaks | No narrative arc; doesn't know who you are; gamification ≠ strategy |
| Journaling apps | Reflection space | No structure; no output; nothing proposed; no memory across entries |
| ChatGPT | Smart, fast | No persistent model that reliably circles backs on your goals |
| Therapist / life coach | Deep insight | Expensive; not available at 11pm; doesn't track your weekly data |
| Goal-setting frameworks (OKRs, SMART) | Structured planning | Static; no one checks in weekly; doesn't adapt to your energy or capacity |

This system is the **only one that combines persistent memory + adaptive planning calibrated to your energy + personalized concern handling based on your failure modes + multi-year arc tracking** — in something that takes 15 minutes a week and lives in your editor.

---

## What gets tracked

- **Weekly:** gym sessions, diet days, social exposures, conversations initiated, grow target progress, energy level, fun activity
- **Monthly:** Survive/Sustain/Grow targets, Role Compass (career clarity), project status, milestone progress
- **Annually:** Strength baselines, pillar trends, habit stack history, project completions
- **Always:** Your vision, your 1-year goals, your "anchor + constellation" life structure

**No daily logging required.** The system infers what it can from weekly inputs and asks only for what it can't compute.

---

## Getting started

### Prerequisites
- [Cursor](https://cursor.com) (the AI code editor — free tier works)
- 30 minutes for quick setup, or ~2 hours for deep setup (the `start` command supports both)

### Setup

1. Clone or fork this repository
2. Open the folder in Cursor
3. Type `start` in a new chat

The `start` command will now do two things in sequence:
- **Technical setup:** confirms your rules/files are in place, verifies personal-data protections in `.gitignore`, and helps with optional Notion MCP setup
- **Life Arc setup:** builds your personal vision, pillars, baselines, and 1-year goals via guided questions

At the end, it generates your `Life-Arc-Overview.md`, which becomes the AI's permanent reference for every future session.

You can choose:
- **Quick setup (~30 min):** enough to start weekly check-ins immediately
- **Deep setup (~2 hours):** stronger baseline detail and clearer milestones

After setup, your weekly workflow is:
- **Every week:** `weekly check-in` (15 min)
- **End of each month:** `monthly reset` (60 min)
- **Every quarter:** self-led review using your logs

---

## Publish safely to GitHub

This project is designed to be shared without exposing your personal goals or progress.

Before your first push, run:

```bash
git init
git add .
git status
```

Review `git status` and confirm personal files are **not** staged:
- `Life-Arc-Overview.md`
- `System/Progress-Log.md`
- `System/Progress-Visualizations.md`
- `System/Role-Compass-Log.md`
- `System/Reflections-Log.md`
- `System/Monthly-Plans/YYYY-*.md`
- `System/Data/monthly-history/*`
- `*.docx`

Then commit and push to your new GitHub repo:

```bash
git commit -m "Initial public template"
git branch -M main
git remote add origin <your-repo-url>
git push -u origin main
```

---

## File structure

```
Life Building/
├── README.md                          ← you are here
├── Life-Arc-Overview.md               ← your north star (generated by `start`)
├── System/
│   ├── Progress-Log.md                ← weekly scoreboard + monthly summaries
│   ├── Progress-Visualizations.md     ← bar charts, habit stack, milestone Gantt
│   ├── Project-Tracker-TEMPLATE.md    ← copy to Project-Tracker.md locally (personal; gitignored)
│   ├── Role-Compass-Log.md            ← monthly career clarity answers
│   ├── Reflections-Log.md             ← deep-dive summaries from Part 5 check-ins
│   ├── Monthly-Plans/
│   │   ├── TEMPLATE-Plan.md           ← blank monthly plan template
│   │   └── YYYY-MM-Plan.md            ← one file per month (auto-created)
│   └── Data/
│       └── monthly-history/           ← structured monthly records (JSON + NDJSON)
└── .cursor/
    └── rules/
        ├── start.mdc                  ← life arc setup command
        ├── weekly-checkin.mdc         ← weekly check-in protocol
        ├── monthly-reset.mdc          ← monthly reset protocol
        ├── concern-handling.mdc       ← stuck? this handles it
        └── depth-breadth.mdc         ← breadth vs. anchor triage
```

---

## Philosophy

This system is built on a few ideas that most productivity tools ignore:

**1. The past as anchor.** You are more motivated by seeing a gap between where you've been and where you need to go than by abstract future goals. This system keeps history visible.

**2. Concern handling over motivation.** When you don't want to do something, the problem is usually an unaddressed objection — not lack of discipline. The `concern handling` command works through every objection until none remain — and after setup, it does this using *your* documented failure modes, not a generic script.

**3. The anchor + constellation model.** You don't need to be excellent at everything. You need to be solid in one thing (the anchor: your career, your craft) and interesting in many (the constellation: fitness, relationships, curiosity, culture). The anchor funds the constellation. This system tracks both without collapsing one into the other.

**4. Capacity is not fixed.** A system that expects the same output from you every week will fail. High-energy weeks, crash periods, chaotic life circumstances — all of these change what's realistic. This system adjusts proposals to your energy level each week, and has a built-in crash mode for genuine low periods.

**5. Systems over willpower.** Willpower is finite and unreliable. This system is designed to require as little of it as possible — through lightweight check-ins, pre-set frameworks, and an AI that has already done the interpretation before you arrive.

**6. Partial progress is progress.** The Progress Log records partial completion. Monthly resets frame incomplete targets as "continuing," not "failed." The system is designed to be honest without being punishing.

---

## Privacy

All data lives locally in your markdown files. Nothing is sent anywhere except to the AI model you configure in Cursor (same as any Cursor conversation). No accounts. No subscriptions. No cloud sync unless you add it yourself.

This repo is configured so personal files are not uploaded by default:
- Personal logs, plans, and life arc files are ignored via `.gitignore`
- Historical monthly data is ignored
- Personal curriculum `.docx` files are ignored

---

## Contributing

This system was built for one person's life. If you use it, your life will look different — different pillars, different anchors, different goals. The `start` command is designed to generate a system tailored to you, not a copy of the original.

If you build something useful — a new rule, an improved question flow, a better visualization format — PRs are welcome.

---

*Built in Cursor. Runs on markdown and AI. Takes 15 minutes a week.*
