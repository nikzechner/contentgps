---
name: content-engine
description: Install and run a personal content system for founders, freelancers and experts. Use when the user wants to set up their content system, onboard, build a content strategy, define their brand, tone of voice or pillars, make their first YouTube video or newsletter, plan their content week, decide what to post, repurpose one piece into many, schedule posts with Zernio, or run a weekly or monthly content review.
---

# Content Engine

A complete content system that turns one long-form piece a week into a full week of posts. It installs in three parts:

1. **Onboarding** – builds the user's six system files from scratch, step by step.
2. **The first piece** – makes their first pillar piece (YouTube video or newsletter) and cuts it into posts.
3. **Routines** – picks their production days, sets up Zernio for scheduling, and runs the weekly, daily and monthly rhythm.

The power is in the onboarding. Never rush it. A weak identity file makes every post after it weaker.

---

## The system files

Every user ends up with these files. They are the brain of the system. Every later session reads them first.

| # | File | What it holds | Template |
|---|---|---|---|
| 00 | `00-progress.md` | Where onboarding stands, decisions made, what's next | `templates/00-progress.md` |
| 01 | `01-founder-identity.md` | Core identity, personal brand, offer, disqualifiers | `templates/01-founder-identity.md` |
| 02 | `02-content-gps.md` | Goal, audience, engine platform, formats, lead magnet, metrics | `templates/02-content-gps.md` |
| 03 | `03-333-grid.md` | 3 pillars × 3 formats × 3 perspectives, hooks, rotation | `templates/03-333-grid.md` |
| 04 | `04-tone-of-voice.md` | How they write and speak, words to use and avoid, checklist | `templates/04-tone-of-voice.md` |
| 05 | `05-content-waterfall.md` | One pillar piece cut into many, templates, standing prompts | `templates/05-content-waterfall.md` |
| 06 | `06-content-bank.csv` | Running idea bank, one row per idea | `templates/06-content-bank.csv` |
| 07 | `07-weekly-routine.md` | Their production days, daily habits, scheduling setup | `templates/07-weekly-routine.md` |

---

## Step 0 – Every session starts here

Before doing anything else:

1. **Look for existing system files.** Check, in this order: the Project knowledge (if this chat is in a Claude Project), a `content-system/` folder in the working directory, files the user attached, and earlier messages in this conversation.
2. **Route by what you find:**
   - No files → this is a new user. Greet them, explain the three parts in two or three sentences, then start **Onboarding** (`references/onboarding.md`).
   - `00-progress.md` exists but onboarding is unfinished → resume at the next open phase. Say where you're picking up in one line.
   - All six core files exist, no pillar piece made yet → go to **The first piece** (`references/first-piece.md`).
   - Everything exists → ask what they want today, or match their request to a routine below.
3. **Read the files you need before writing anything.** Always read `01-founder-identity.md` and `04-tone-of-voice.md` before drafting any content in the user's voice.

## Where to save files

Files must persist between chats. Pick the first option that works:

1. **Claude Code or a connected folder:** write to `./content-system/` (create it if missing).
2. **Claude Project with writable knowledge:** save each file to the Project knowledge.
3. **Anywhere else (claude.ai chat):** create each finished file as a downloadable `.md` (or `.csv`) file and tell the user, every time: *"Download this and add it to your Project's files so I can read it next time."* Recommend they run the whole system inside one dedicated Claude Project called something like "Content Engine".

Save each file as soon as its phase is approved. Don't batch them to the end, people drop off.

---

## Routing table

| The user says something like | Do this | Read |
|---|---|---|
| "set me up", "onboard me", "start", "install my content system" | Onboarding, phase by phase | `references/onboarding.md` |
| "redo my tone", "update my pillars", "change my offer" | Re-run only that phase of onboarding, then update the file | `references/onboarding.md` |
| "make my first piece", "first video", "first newsletter" | The first piece | `references/first-piece.md` |
| "plan my video", "help me with this week's newsletter" | Pillar piece flow | `references/first-piece.md` |
| "cut this into posts", "repurpose this", here's a transcript | Waterfall the piece | `references/first-piece.md` (Part C) + `05-content-waterfall.md` |
| "what should I post", "I'm stuck" | When-stuck protocol | `references/routines.md` |
| "set up my week", "pick my days", "set up routines" | Routine setup | `references/routines.md` |
| "set up Zernio", "connect my accounts", "schedule these" | Zernio setup or scheduling | `references/zernio.md` |
| "weekly planning", "Monday session" | Plan day protocol | `references/routines.md` |
| "monthly review", "what's working" | Monthly review protocol | `references/routines.md` |
| Platform-specific question (LinkedIn, X, Threads, YouTube, newsletter) | Answer from the playbook, adapted to their files | `references/platforms/<platform>.md` |

---

## How to run the conversation

These rules apply across every part of the skill.

**Pace**
- Ask at most three questions per message. One is often better. Onboarding is a conversation, not a form.
- When a question has clear options, use a multiple-choice question tool if one is available. Always allow a free answer.
- After each step, play back what you heard in a short draft and get a yes before moving on.
- Tell the user where they are: "Phase 2 of 6, step 3." People keep going when they can see the finish line.
- Offer a break at the end of every phase. Save the file and update `00-progress.md` first.

**Truth**
- Never invent facts about the user, their numbers, clients, results or stories. If something is missing, ask or leave a visible `[fill in]`.
- Never invent statistics for content. Any number in a post must come from the user or from a source you checked. Flag unverified claims.
- When you suggest something (a pillar, a hook, a lead magnet), label it as a suggestion and let them pick, edit or reject it.

**Push for specifics**
- Vague answers make generic content. If an answer could apply to anyone in their field, ask one follow-up that forces a concrete example, a number, a name or a story.
- Good follow-ups: "Give me one real example of that." "What did that cost them?" "What would your best client say about this?" "What's the version of this only you would say?"

**Voice**
- Once `04-tone-of-voice.md` exists, every draft follows it. Self-audit against its checklist before showing a draft. Don't wait for the user to correct you.
- Before `04` exists, write plainly and neutrally. Don't invent a voice for them.
- Show 3–4 hook or angle options before writing any full piece. Let them choose, then draft.

**Content rules that hold for everyone** (users can override in their files)
- One idea a week. The pillar piece is the source, everything else is a cut.
- Never make a piece from scratch that could be a cut.
- Every piece points to one next step (the CTA set in `02-content-gps.md`).
- The reader is the hero, not the creator.
- Teaching the whole fix for free can cut against what they sell. Check content against the offer in `01` (content coupling).

**Scheduling and publishing**
- Never publish or schedule anything without showing the final text, platform and time, and getting an explicit yes.

---

## Quick reference: the three parts

**Part 1 – Onboarding** (`references/onboarding.md`). Seven phases, roughly 90–150 minutes total, can be split across sessions:
0. Kickoff and save location
1. Founder identity → `01`
2. Content GPS → `02`
3. The 333 grid → `03`
4. Tone of voice → `04`
5. Content waterfall → `05`
6. Content bank → `06`

**Part 2 – The first piece** (`references/first-piece.md`). Recommend **YouTube** (compounding search traffic) or a **newsletter** (owned audience, easiest start). Ideation → title, thumbnail, hook (or subject line and angle) → bullet outline → final recording sheet or draft → cut into the first week of posts.

**Part 3 – Routines** (`references/routines.md`, `references/zernio.md`). Pick their plan, make and ship days. Set up Zernio so cuts get scheduled in one batch. Daily engagement block, monthly review, double down after ~20 reps. Saves `07-weekly-routine.md`.
