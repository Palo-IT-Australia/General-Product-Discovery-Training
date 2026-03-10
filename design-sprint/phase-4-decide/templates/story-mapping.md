> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides the group through each step, collects input via Copilot Chat, and populates this document progressively. Do not edit manually during a live session.

**Activity type:** Group | **Time:** 60–90 minutes | **Sprint phase:** Phase 4 — Decide

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

Story Mapping breaks the solution selected during Phase 4 into individual, workable user stories — small, concrete units of value that can be built and tested independently. Organised around the user's journey, the map makes it immediately clear what to prototype and in what order.

Each story is then scored using the **RICE prioritisation method** to ensure the team focuses first on stories that deliver the most value relative to the effort required.

| RICE Factor | What it measures | Scale |
|---|---|---|
| **Reach** | How many users will this story affect per sprint/month? | Estimated number or 1–10 |
| **Impact** | How much will this improve the experience for those users? | 3 = massive · 2 = high · 1 = medium · 0.5 = low · 0.25 = minimal |
| **Confidence** | How confident are we in the Reach and Impact estimates? | 100% = high · 80% = medium · 50% = low |
| **Effort** | How many person-weeks does this story require end-to-end? | Person-weeks (higher = more effort) |

**RICE Score formula:**

$$\text{RICE Score} = \frac{\text{Reach} \times \text{Impact} \times \text{Confidence}}{\text{Effort}}$$

A higher RICE score means higher priority.

**Example:**
Story: *"Show AI-suggested follow-up message to the sales agent before sending"*
→ Reach: *8* · Impact: *2* · Confidence: *80%* · Effort: *2 weeks*
→ RICE Score: *(8 × 2 × 0.8) / 2 = **6.4***

---

## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run Story Mapping`

---

## Step 1 — Load Sprint Context

**What the agent does:** Reads the Problem Statement from Phase 2 and the Storyboard from the current phase, then presents both to the group to anchor the session.

> **Agent prompt to group:**
> *"Before we map stories, let's anchor on our two key inputs. Here is the Problem Statement and the Storyboard we produced earlier in this sprint. Read both, then confirm you're ready to proceed. Reply `ready` when the group is aligned."*

| Input | Content |
|---|---|
| Problem Statement | _(DesignSprintAgent pulls from `phase-2-define/problem-statement.md`)_ |
| Chosen Solution (from Storyboard) | _(DesignSprintAgent pulls from `phase-4-decide/storyboard.md`)_ |

---

## Step 2 — Identify User Activities (Backbone)

**What the agent does:** Prompts the group to identify the high-level user activities that form the backbone of the story map — the major steps the user takes to move from their starting point to their goal.

> **Agent prompt to group:**
> *"Let's build the backbone of our story map — the major activities a user goes through when using this solution, from first touchpoint to successful outcome. Think of these as the chapters in the user's story. Aim for 4–7 activities. Reply using this format, one per line:*
> `[Your name]: Activity — {activity name}: {one-sentence description}`"*

| # | Activity Name | Description |
|---|---|---|
| 1 | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |

---

## Step 3 — Break Down into User Stories

**What the agent does:** For each backbone activity, prompts the group to brainstorm the individual user stories — the specific tasks, features, or interactions the user needs to complete that activity. Records all stories against their parent activity.

> **Agent prompt to group:**
> *"Now let's break each activity down into individual user stories — the specific things a user needs to be able to do within that activity. Write each story in the format: 'As a [user], I want to [action] so that [outcome]'. Prefix each story with the activity number it belongs to. Reply using this format:*
> `[Your name]: Activity {#} — As a {user}, I want to {action} so that {outcome}`"*

| Story ID | Parent Activity | User Story | Answers Problem Statement? |
|---|---|---|---|
| S-01 | _(activity name)_ | _(DesignSprintAgent fills in)_ | _(Yes / Partially / No)_ |
| S-02 | | | |
| S-03 | | | |
| S-04 | | | |
| S-05 | | | |
| S-06 | | | |
| S-07 | | | |
| S-08 | | | |

---

## Step 4 — RICE Scoring

**What the agent does:** Presents each story one at a time and asks the group to score it on Reach, Impact, Confidence, and Effort. Calculates the RICE score automatically and records results.

> **Agent prompt to group:**
> *"We'll now score each story using RICE. For each story I present, reply with four numbers in this format:*
> `[Your name]: R={reach 1-10} I={impact: 3/2/1/0.5/0.25} C={confidence: 100/80/50} E={effort in person-weeks}`
> *We'll average the group's scores for each story."*

| Story ID | User Story (short) | Reach (R) | Impact (I) | Confidence (C) | Effort (E) | RICE Score |
|---|---|---|---|---|---|---|
| S-01 | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(R × I × C / E)_ |
| S-02 | | | | | | |
| S-03 | | | | | | |
| S-04 | | | | | | |
| S-05 | | | | | | |
| S-06 | | | | | | |
| S-07 | | | | | | |
| S-08 | | | | | | |

---

## Step 5 — Prioritised Story List

**What the agent does:** Sorts all stories by RICE score (descending) and presents the prioritised backlog to the group. Asks the group to confirm or adjust the order, and to mark which stories form the **Prototype Slice** — the minimum set that will be prototyped to answer the Problem Statement.

> **Agent prompt to group:**
> *"Here is the prioritised story list ranked by RICE score. Review it as a group. Are there any stories you'd like to move up or down? Once you're aligned, tell me which stories should be in the Prototype Slice — the minimum set we need to prototype to answer our Problem Statement. Reply using this format:*
> `[Your name]: Prototype Slice — S-{nn}, S-{nn}, S-{nn}`"*

| Priority | Story ID | User Story (short) | RICE Score | Prototype Slice? |
|---|---|---|---|---|
| 1 | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(✅ Yes / ⬜ No)_ |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |
| 6 | | | | |
| 7 | | | | |
| 8 | | | | |

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to the Prototype phase.)*

| Field | Value |
|---|---|
| Problem Statement Addressed | _(DesignSprintAgent fills in — confirm the Problem Statement that anchored the session)_ |
| Total Stories Generated | _(DesignSprintAgent fills in)_ |
| Prototype Slice Stories | _(DesignSprintAgent fills in — list of Story IDs selected for prototyping)_ |
| Highest RICE Score Story | _(DesignSprintAgent fills in — story ID and score)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important discovery about scope, complexity, or user need that emerged)_ |

### Feed-forward to Prototype

The Prototype Slice and Story Map directly shape what to build in the Prototype phase:

| Prototype Planning Field | How this activity informs it |
|---|---|
| **Prototype Scope** | Only stories marked as Prototype Slice should be included in the prototype build — scope anything else out |
| **Feature Priority** | Use RICE rank order to decide which feature to build first if time is limited |
| **Success Criteria** | Each story's "so that {outcome}" clause defines what the prototype interaction must demonstrate |
| **Problem Statement Validation** | Stories marked "Answers Problem Statement? = Yes" are the critical flows the prototype must test |

> **Suggested Prototype focus** *(generated by DesignSprintAgent from the Prototype Slice)*:
>
> _(DesignSprintAgent generates a one-paragraph prototype brief here, summarising which stories to build and what user outcome each must demonstrate)_

---

## Notes & Observations

> *(Tensions surfaced during the session, stories deprioritised due to effort, dependencies between stories, dissenting views, or follow-up actions the group identified.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take the Prototype Slice and Session Summary into the **Prototype** phase.
> The prioritised story list and RICE scores provide the build order and acceptance criteria for each prototype screen.
