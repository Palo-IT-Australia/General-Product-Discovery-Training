> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides the group through each step, collects input via Copilot Chat, and populates this document progressively. Do not edit manually during a live session.

**Activity type:** Individual (simultaneous) | **Time:** 15–20 minutes | **Sprint phase:** Phase 3 — Sketch
**Source:** [Jake Knapp](https://jakeknapp.com) via [Google Design Sprint Kit](https://designsprintkit.withgoogle.com/methodology/overview)

---

## Session Details

| Field | Value |
|---|---|
| Date | _(DesignSprintAgent fills in)_ |
| Participants | _(DesignSprintAgent fills in from introductions)_ |
| Sprint Context | _(DesignSprintAgent fills in from sprint tracker)_ |
| Facilitator | DesignSprintAgent |

---

## About This Activity

Crazy 8s is a rapid, individual sketching exercise designed to break fixation on the first idea that comes to mind. Each participant sketches 8 distinct ideas in 8 minutes — one idea per panel, one minute per panel. Speed is intentional: it forces divergent thinking and prevents overthinking.

The output is not polished art — it is a wide variety of candidate ideas that the group can then evaluate together. Even a rough box with an arrow tells a story. Crazy 8s is most powerful when participants give each panel a genuinely different idea, rather than 8 variations of the same concept.

| Crazy 8s Mindset | What to Avoid |
|---|---|
| Quantity over quality — generate as many ideas as possible | Polishing one idea across multiple panels |
| Wild ideas are welcome — they spark better real ones | Waiting for the "right" idea before drawing |
| Every panel must be meaningfully different | Variations of the same core concept |
| Stick figures and boxes are enough | Stopping because you "can't draw" |

**Example:**
Problem Statement: *"Busy HR managers need a way to track onboarding completion without manual follow-up, because missed steps delay new hire start dates."*
→ Panel 1: *Automated daily Slack reminder to new hire with checklist progress bar*
→ Panel 2: *HR manager dashboard with traffic-light status per new hire*
→ Panel 3: *New hire mobile app with step-by-step onboarding wizard*
→ Panel 4: *Auto-escalation email to manager if Day 3 tasks not complete*
→ … *(and so on — each a genuinely different mechanism)*

---

## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run Crazy 8s`

---

## Step 1 — Anchor on the Problem Statement

**What the agent does:** Reads the Problem Statement from `design-sprint/phase-2-define/problem-statement.md` and presents it to the group. Confirms everyone has it in mind before starting the sketch round. Also shares the North Star Goal from the Product Brief as an additional anchor.

> **Agent prompt to group:**
> *"Before we sketch, let's anchor on the problem we're solving. Here is the Problem Statement from Phase 2:*
>
> *[Problem Statement is displayed here by the agent]*
>
> *Keep this in mind as you sketch — every idea you draw should be a direct response to this problem. Reply `ready` when everyone is set."*

| Input | Content |
|---|---|
| Problem Statement | _(DesignSprintAgent pulls from `phase-2-define/problem-statement.md`)_ |
| Target User | _(DesignSprintAgent pulls from Problem Statement or User Persona)_ |

---

## Step 2 — Solo Sketch Round (8 panels, 8 minutes)

**What the agent does:** Announces the start of the timed sketch round. Explains the format and ground rules, then starts the clock. The agent waits silently — no prompts during sketching. After 8 minutes, signals time is up.

> **Agent prompt to group:**
> *"Time for Crazy 8s! Here are the rules:*
> *— Fold a piece of paper into 8 panels (fold in half 3 times).*
> *— You have 8 minutes total: 1 minute per panel.*
> *— Each panel = one distinct idea for how to solve the Problem Statement.*
> *— Stick figures, boxes, and arrows are perfectly fine — communicate the concept, not the design.*
> *— Each panel must be a genuinely different approach, not a variation of the same idea.*
>
> *I'll be silent during the sketch. Reply `done` when your 8 minutes are up — we'll move to sharing."*

> **Timer:** *(DesignSprintAgent notes the start time here and confirms when 8 minutes have elapsed)*

---

## Step 3 — Share and Present Ideas

**What the agent does:** Asks each participant to briefly describe all 8 of their ideas out loud (or in chat), giving a one-sentence explanation per panel. Records each participant's ideas in the table below. No critique or feedback is given at this stage — the goal is just to surface what was generated.

> **Agent prompt to group:**
> *"Let's hear what everyone sketched. Go one at a time — describe each of your 8 panels in a sentence or two. Don't explain or defend them yet; just tell us what each idea is.*
> Reply using this format, one panel per line:*
> `[Your name] Panel [1–8]: {one-sentence description of the idea}`"*

| Participant | Panel | Idea Description |
|---|---|---|
| _(DesignSprintAgent fills in)_ | 1 | _(DesignSprintAgent fills in from chat responses)_ |
| | 2 | _(DesignSprintAgent fills in)_ |
| | 3 | _(DesignSprintAgent fills in)_ |
| | 4 | _(DesignSprintAgent fills in)_ |
| | 5 | _(DesignSprintAgent fills in)_ |
| | 6 | _(DesignSprintAgent fills in)_ |
| | 7 | _(DesignSprintAgent fills in)_ |
| | 8 | _(DesignSprintAgent fills in)_ |

*(Repeat the above block for each participant)*

---

## Step 4 — Identify Strongest Ideas

**What the agent does:** Asks each participant to nominate their own strongest 1–2 ideas from their 8 panels. Records nominations. These become the candidates for the Solution Sketch activity (if chosen) or are carried forward directly to Phase 4 as inspiration for the Storyboard.

> **Agent prompt to group:**
> *"Now that everyone has shared, choose your own best 1–2 ideas from your 8 panels — the ones you feel most strongly solve the Problem Statement. You don't need to justify them yet.*
> Reply using:*
> `[Your name]: My top idea(s) — Panel [number(s)]: {brief recap of the idea}`"*

| Participant | Top Idea(s) | Panel # | Why It's Strong |
|---|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in from chat responses)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in if participant offered a reason)_ |
| | | | |

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to Solution Sketch or Phase 4.)*

| Field | Value |
|---|---|
| Total Ideas Generated | _(DesignSprintAgent fills in — participants × 8)_ |
| Ideas Nominated as Top | _(DesignSprintAgent fills in — total nominations across all participants)_ |
| Most Common Theme | _(DesignSprintAgent fills in — any pattern or cluster visible across participants' top ideas)_ |
| Most Divergent Idea | _(DesignSprintAgent fills in — the idea that least resembles the others, worth noting)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important direction or tension that emerged across the group's ideas)_ |

### Feed-forward to Solution Sketch

The strongest ideas identified in Step 4 become the starting point for the Solution Sketch activity:

| Solution Sketch Field | How this activity informs it |
|---|---|
| **Solution Title** | Each participant's top idea from Step 4 becomes the title of their Solution Sketch |
| **Problem Being Solved** | Anchored on the same Problem Statement used in Step 1 |
| **Panel 1 — Context/Entry** | The trigger or starting condition sketched in the Crazy 8s panel |
| **Panel 2 — Core Interaction** | The mechanism of the idea sketched in the Crazy 8s panel |
| **Panel 3 — Outcome** | The end state implied by the Crazy 8s idea |
| **Key Assumptions** | The assumptions that made this idea feel promising in 1 minute of sketching |

> **Suggested Solution Sketch focus** *(generated by DesignSprintAgent from the group's top ideas)*:
>
> _(DesignSprintAgent generates a suggested framing here, e.g. "The most-nominated direction was [theme] — this suggests the Solution Sketch round should explore [direction] in more depth.")_

---

## Notes & Observations

> *(Ideas that surprised the group, recurring themes worth noting, ideas deliberately set aside that might be worth revisiting, tensions between participants' directions.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take the top ideas into the **Solution Sketch** activity to develop the strongest one into a detailed 3-panel story.
> Invoke `@DesignSprintAgent let's run Solution Sketch` to continue Phase 3.
