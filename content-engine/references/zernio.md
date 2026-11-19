# Zernio: setup and scheduling

Zernio is a social media scheduler with a hosted MCP server. Once connected, Claude can create, schedule and check posts across LinkedIn, X, Threads, Instagram, YouTube, TikTok, Facebook and more, straight from the chat. It means Ship day ends with everything scheduled in one batch.

Product details change. If a step below doesn't match what the user sees, check https://docs.zernio.com/mcp/setup.

---

## Part 1 – Setup (10–15 min)

### Step 1 – Create the account

1. Go to https://zernio.com and sign up.
2. In the dashboard, create a **profile** (one profile per brand; most solo users need one).
3. **Connect the social accounts** from `02-content-gps.md` (engine + distribution platforms). Only connect the ones they'll actually post to.

### Step 2 – Connect Zernio to Claude

**Claude (web, desktop or mobile app):**
1. Open **Settings → Connectors**.
2. Choose **Add custom connector**.
3. Name: `Zernio`. URL: `https://mcp.zernio.com/mcp`.
4. Click **Add**, then sign in with the Zernio account when Claude redirects. No API key needed.
5. In a new chat (inside their Content Engine Project), make sure the Zernio connector is switched on.

**Claude Code:**
```bash
claude mcp add --transport http zernio https://mcp.zernio.com/mcp
```
Then run `/mcp` inside Claude Code and sign in.

### Step 3 – Verify

Ask Claude to list the connected Zernio accounts. Each connected platform should show up with its username. If it says no accounts are connected, go back to Step 1.3.

**Common fixes**
- "Couldn't reach the MCP server" or sign-in errors: remove the connector and add it again.
- 401 errors: remove and re-add the connector to rerun sign-in.
- Changes not showing: fully restart the Claude app.

### Step 4 – Best times

If Zernio's analytics have enough history, fetch the best times to post per platform and suggest them. If not, use these defaults until there's data, and write them into `07-weekly-routine.md`:
- LinkedIn: weekdays, 8–10am in the buyers' time zone. Avoid evenings.
- X: 1–2 posts a day, spaced at least 4–5 hours apart.
- Threads: 1–2 posts a day, when the user can be online for the first 30–60 minutes to reply.

---

## Part 2 – Scheduling on Ship day

1. **Collect the approved pieces** from the waterfall. Only pieces the user has explicitly approved.
2. **Build the schedule** as a table: Platform | Day | Time | First line of the post | Media | Link placement.
3. **Check the rules** per platform from `references/platforms/`:
   - Spacing between posts on the same platform.
   - Links in the first comment or reply, not the post body, where the playbook says so. If first-comment scheduling isn't supported for that platform, list those comments for the user to post manually.
   - Media attached where planned (before/after images, clips). Upload media through Zernio's media tools if needed.
4. **Show the full schedule and get an explicit yes.** Never schedule or publish without it.
5. **Validate, then schedule.** Use Zernio's validation where available, then create the scheduled posts.
6. **Confirm back** with what got scheduled, where and when, and anything that failed.
7. **Log** in the content bank.

### Checking in

- During the week: if asked, list scheduled and failed posts. Offer to retry failed ones after showing what will be retried.
- Monthly review: pull post analytics per platform to fill the Result column.

---

## Without Zernio

If the user doesn't want Zernio, give them the pieces in posting order with suggested day and time per platform, and point them to each platform's native scheduler. The rest of the system works the same.
