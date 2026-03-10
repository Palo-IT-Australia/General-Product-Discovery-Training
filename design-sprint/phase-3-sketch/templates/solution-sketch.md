> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides each participant in developing their strongest idea and saves one artefact per participant. Do not edit manually during a live session.

**Activity type:** Individual | **Time:** 30–45 minutes | **Sprint phase:** Phase 3 — Sketch
**Source:** [Google Design Sprint Kit](https://designsprintkit.withgoogle.com/methodology/overview)

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

The Solution Sketch takes the best idea from the sketch phase — whether generated through Crazy 8s or developed independently — and expands it into a detailed, annotated 3-panel story. Unlike Crazy 8s, which values breadth and speed, the Solution Sketch values depth and clarity.

A good Solution Sketch should be self-explanatory: someone who was not in the room should be able to read it and understand exactly what the solution is, who it is for, and what value it delivers — without needing to ask any questions. This level of detail is what makes it possible to evaluate, vote on, and storyboard the solution in Phase 4.

Each participant creates their own Solution Sketch. The agent saves one artefact file per participant: `solution-sketch-[author-slug].md`.

| Solution Sketch | What to Avoid |
|---|---|
| Focused on one specific idea developed in depth | Trying to combine multiple ideas into one sketch |
| Self-explanatory without the author present | Vague descriptions that require verbal explanation |
| Grounded in the Problem Statement | Solving a different problem than the one defined in Phase 2 |
| Annotated with enough detail to prototype | Artistic quality — clarity of thought matters, not drawing skill |

**Example:**
Idea (from Crazy 8s): *"HR dashboard with traffic-light status per new hire"*
→ Panel 1: *"HR manager opens the onboarding dashboard on Monday morning. She sees a list of all active new hires with colour-coded status (green = on track, amber = 1+ tasks overdue, red = 3+ tasks overdue). No manual checking needed."*
→ Panel 2: *"She clicks on a red status. The system shows exactly which tasks are overdue, since when, and offers a one-click 'Send Reminder' button that auto-populates a message to the new hire and their line manager."*
→ Panel 3: *"By end of day, the overdue tasks are completed. The status turns green. HR receives no escalation emails and spends 0 minutes on manual follow-up for that new hire."*

---

## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run Solution Sketch`

---

## Step 1 — Choose the Idea to Develop

**What the agent does:** Anchors on the Problem Statement and asks each participant to nominate the idea they will develop into their Solution Sketch. If Crazy 8s was completed, prompts them to draw from their top Crazy 8s ideas.

> **Agent prompt to group:**
> *"Each person will now develop one idea into a detailed Solution Sketch. Choose the idea you feel most strongly addresses the Problem Statement — this can come from your Crazy 8s top picks, or from an idea that emerged during the sharing conversation.*
>
> *Problem Statement: [Agent reads from `phase-2-define/problem-statement.md`]*
>
> *Tell me which idea each of you is developing. Reply using:*
> `[Your name]: I'm sketching — {one-sentence description of the idea you're developing}`"*

| Participant | Idea Being Developed |
|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in from chat responses)_ |
| | |

---

## Step 2 — Develop the 3-Panel Story

**What the agent does:** Guides each participant through describing their solution as a 3-panel story — Context/Entry, Core Interaction, and Outcome. Collects each panel description in chat and records it. Creates a separate artefact file `solution-sketch-[author-slug].md` for each participant using steps 2–4 as the content.

> **Agent prompt to group:**
> *"Now describe your solution as a 3-panel story — write it as if narrating a short film for your target user. One panel at a time:*
>
> *Panel 1 — What is happening before the user interacts with your solution? What is the trigger or the context? What is the user's state of mind?*
>
> *Reply using: `[Your name] Panel 1: {your description}`"*
>
> *(Agent collects Panel 1 for all participants, then repeats for Panel 2 and Panel 3)*

> **Agent prompt for Panel 2:**
> *"Panel 2 — What does the user do, and how does your solution respond? Describe the core interaction step-by-step. What does the user see, click, say, or do? What does the system show or do in response? Be specific enough that someone could prototype this without asking you any questions.*
>
> *Reply using: `[Your name] Panel 2: {your description}`"*

> **Agent prompt for Panel 3:**
> *"Panel 3 — What is the outcome for the user? What has changed? What value have they received? How does this directly address the pain identified in Phase 1?*
>
> *Reply using: `[Your name] Panel 3: {your description}`"*

---

## Solution Sketch: _(Solution Title)_

**Author:** _(DesignSprintAgent fills in)_
**Date:** _(DesignSprintAgent fills in)_
**Inspired by:** _(DesignSprintAgent fills in — Crazy 8s panel number, or HMW note that sparked this idea)_

---

### Problem Being Solved

> _(DesignSprintAgent fills in — one sentence: which aspect of the Problem Statement does this solution address?)_

---

### Panel 1 — Context / Entry Point

**What happens before the user interacts with this solution?**

_(DesignSprintAgent fills in from participant's Panel 1 response — trigger, context, and user's state of mind)_

---

### Panel 2 — Core Interaction

**What does the user do, and how does the solution respond?**

_(DesignSprintAgent fills in from participant's Panel 2 response — step-by-step interaction, what the user sees/does, what the system shows/does)_

---

### Panel 3 — Outcome

**What is the result for the user?**

_(DesignSprintAgent fills in from participant's Panel 3 response — end state, value delivered, connection back to the pain point)_

---

## Step 3 — Key Assumptions and Open Questions

**What the agent does:** Prompts each participant to surface the assumptions their solution rests on, and any open questions that would need to be resolved before prototyping. Records both.

> **Agent prompt to group:**
> *"Two final inputs for your sketch: (1) What must be true for your solution to work? List 2–3 assumptions you're making. (2) What is still unknown or unresolved?*
>
> *Reply using:*
> `[Your name] Assumption [1/2/3]: {assumption}`*
> `[Your name] Question [1/2]: {open question}`"*

### Key Assumptions

| # | Assumption |
|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in from participant responses)_ |
| | |

### Open Questions

| # | Question |
|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in from participant responses)_ |
| | |

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to Phase 4 — Decide.)*

| Field | Value |
|---|---|
| Total Solution Sketches Completed | _(DesignSprintAgent fills in)_ |
| Artefact Files Created | _(DesignSprintAgent fills in — list of `solution-sketch-[author-slug].md` file paths)_ |
| Most Common Solution Direction | _(DesignSprintAgent fills in — if a theme emerges across sketches)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important design direction or tension that emerged across the sketches)_ |

### Feed-forward to Storyboard (Phase 4)

The Solution Sketches are the primary input for the Phase 4 Storyboard:

| Storyboard Field | How this activity informs it |
|---|---|
| **Opening Scene** | Panel 1 (Context/Entry) of the winning sketch becomes the storyboard's opening frame |
| **Core Interaction Frames** | Panel 2 (Core Interaction) is expanded into the middle frames of the storyboard |
| **Closing Scene** | Panel 3 (Outcome) becomes the storyboard's closing frame |
| **Key Decisions** | Assumptions and open questions surfaced here become decisions the team resolves during storyboarding |
| **Elements from Other Sketches** | Strong elements from non-winning sketches can be incorporated into the storyboard if the group agrees |

> **Suggested Storyboard starting point** *(generated by DesignSprintAgent from completed sketches)*:
>
> _(DesignSprintAgent generates a suggested opening frame here once all sketches are complete, e.g. "Based on the sketches, the storyboard might open with: '[User] encounters [trigger situation]…'")_

---

## Notes & Observations

> *(Tensions between sketches, strong elements in non-winning sketches worth preserving, open questions that came up repeatedly, observations about divergence or convergence across participants.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take all completed Solution Sketches into **Phase 4 — Decide** to select the strongest solution and build the Storyboard.
> Invoke `@DesignSprintAgent let's move to Phase 4` to begin the Decide phase.
