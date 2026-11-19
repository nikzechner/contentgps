# Content Engine

**Make one piece of content a week. Get 30 posts out of it. In your own voice.**

A free Claude skill that sets up your whole content system for you. Brand, strategy, tone of voice, 12 weeks of ideas, your first video or newsletter, and a weekly routine that schedules everything. You answer questions, Claude builds the system.

**[⬇ Download the skill (content-engine.zip)](./content-engine.zip)** · [Install in 2 minutes](#install)

---

## Sound familiar?

- You know content brings clients. You just never know what to post.
- You post for two weeks, get busy with client work, and disappear for two months.
- AI drafts sound like everyone else on LinkedIn. You rewrite them and it takes longer than writing from scratch.
- You're on five platforms and none of them bring in leads.
- Your audience is full of peers who like your posts and never buy.

Content Engine fixes the system behind that, not just the posts.

---

## What you get

### 1. A full onboarding that builds your strategy with you

This is the part most people skip, and the reason their content feels like effort. Claude interviews you step by step (90 to 150 minutes, pause anytime) and builds six files that become the brain of your content:

| You get | What it does for you |
|---|---|
| **Founder identity** | Lines up who you are, your personal brand, and what you sell, so every post points at your offer |
| **Content GPS** | Your goal in numbers, your ideal buyer, the words they search, your one engine platform, your lead magnet |
| **The 333 grid** | 3 pillars × 3 formats × 3 beliefs. 9 cells, each good for a dozen posts. You never run out of ideas |
| **Tone of voice** | Built from how you actually talk and write. Drafts sound like you, not like a model |
| **Content waterfall** | The exact way one video or newsletter becomes 10 to 30 posts across LinkedIn, X and Threads |
| **Content bank** | 12 weeks of titles and hooks, ready on day one |

### 2. Your first piece, made together

Claude recommends **YouTube** (search traffic that compounds for years) or a **newsletter** (an audience you own), then helps you make the first one: title, thumbnail, hook, outline, recording sheet. Then it cuts it into your first week of posts.

### 3. A routine that runs itself

Pick your plan day, make day and ship day. Claude connects to **Zernio** and schedules every post across your platforms in one batch, straight from the chat. Plus a 15 minute daily engagement habit and a monthly review that tells you what to double down on.

---

## Who it's for

- **Founders** who sell B2B and want content to bring in calls, not likes
- **Freelancers, consultants and agency owners** who need a pipeline without a marketing team
- **Marketers** setting up a founder-led content system for a client or their CEO
- **Experts** with something to say and four hours a week to say it

If you want a viral growth hack, this isn't it. It's built for people playing the long game.

---

## How a week looks once it's running

| Day | Time | What you do |
|---|---|---|
| Plan day | 30 min | "Run my weekly planning session." Claude picks the idea and writes your outline |
| Make day | 2 to 3 h | Record the video or write the newsletter. One take, light edit |
| Ship day | 1 h | "Here's the transcript, run Ship day." Claude cuts it into posts and schedules them |
| Every day | 15 min | Reply to comments. Claude can draft the replies |

About 5 hours a week for a full week of content on every platform you care about.

---

## Install

You need a Claude account (Pro or higher recommended) with **Code execution and file creation** turned on under Settings → Capabilities.

### Option A: Claude app (web or desktop), recommended

1. **[Download content-engine.zip](./content-engine.zip)** (click the file, then the download icon).
2. In Claude, open **Customize → Skills**, click **+**, then **Create skill → Upload a skill**, and pick the zip.
3. Create a new **Project** called `Content Engine`. Your files will live here.
4. Start a chat inside the project and type:

   > **Set up my content engine**

5. Each time Claude finishes a file, add it to the Project's files. That's how Claude remembers you next time.

*Menus move around. If the steps don't match, search "upload a skill" on [support.claude.com](https://support.claude.com).*

### Option B: Claude Code

```bash
git clone https://github.com/nikzechner/contentgps.git
cp -r contentgps/content-engine ~/.claude/skills/
```

Open Claude Code in the folder where you want your files and say **"Set up my content engine"**. Files get saved to `./content-system/`.

### Option C: No skills? Use a Project

1. Create a Claude Project.
2. Upload everything inside the `content-engine/` folder as Project files.
3. Paste this into the Project instructions: `Follow SKILL.md in the project files.`
4. Say **"Set up my content engine"**.

---

## Things to say once it's set up

| Say | What happens |
|---|---|
| "Run my weekly planning session" | Picks this week's idea, gives you title options and an outline |
| "Give me my recording sheet" | Title, hook and bullet points to record from |
| "Here's the transcript, run Ship day" | Cuts it into posts for every platform and schedules them |
| "What should I post?" | Picks from your grid and your bank |
| "Run my monthly review" | Shows what's working and picks one thing to change |
| "Update my tone of voice" | Re-runs just that step |

---

## Connect Zernio (optional, recommended)

1. Sign up at [zernio.com](https://zernio.com), create a profile, connect your social accounts.
2. In Claude: **Settings → Connectors → Add custom connector**. Name `Zernio`, URL `https://mcp.zernio.com/mcp`. Sign in.
3. Say **"Set up Zernio"**. Claude checks the connection and sets your posting times.

Claude never posts or schedules anything without showing you first and getting a yes.

---

## FAQ

**Is it free?**
Yes. MIT license. You need your own Claude plan. Zernio is optional.

**Will it write in my voice or in some guru's voice?**
Yours. Every template ships empty. The tone of voice file is built from samples of how you actually write and talk, then tested until the drafts sound like you.

**Do I need to be on camera?**
No. If you'd rather write, the newsletter becomes your engine. If you do video, screen share works great.

**I don't have time for 90 minutes of onboarding.**
Do it in three 30 minute sittings. Progress is saved. It's the part that makes the next 52 weeks easy.

**Which platforms does it cover?**
YouTube and newsletters as the engine. LinkedIn, X and Threads for distribution, with playbooks for each. Zernio can post to most other platforms too.

---

## What's inside

```
content-engine/
├── content-engine.zip          ← upload this to Claude
└── content-engine/             ← the skill
    ├── SKILL.md
    ├── references/
    │   ├── onboarding.md       ← the step-by-step onboarding
    │   ├── first-piece.md      ← YouTube + newsletter flows, the waterfall
    │   ├── routines.md         ← weekly, daily and monthly sessions
    │   ├── zernio.md           ← scheduling setup
    │   └── platforms/          ← YouTube, newsletter, LinkedIn, X, Threads playbooks
    └── templates/              ← empty files Claude fills in with you
```

---

## Honest notes

- The first 20 pieces matter more than the results. Most people quit before rep 20, which is roughly where it starts working.
- Platform notes were researched in late 2026. Algorithms change, so check numbers before quoting them.
- The frameworks (founder identity, 333 grid, content GPS, waterfall, content bank) are adapted from Matt Gray's content system.

---

Built by **Nik Zechner**. If it helps you, star the repo so more people find it. ⭐

MIT License.
