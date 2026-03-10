> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent simulates a realistic user persona based on the Product Brief, conducts a live interview in Copilot Chat, then synthesises the conversation into structured insights. Do not edit manually during a live session.

**Activity type:** Individual / Pair | **Time:** 10–15 minutes per interview | **Sprint phase:** Phase 1 — Understand
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

**Purpose:** User Interviews exist to challenge assumptions. Instead of the team deciding what users need, interviews let users tell us — in their own words — what frustrates them, what workarounds they have invented, and where they feel things could be better. The goal is to surface **pain points** (what is broken or hard today) and **opportunities** (where improvements would make a real difference), grounded in real experience rather than speculation.

**What great interviewers listen for:**

| Listen for | Avoid |
|---|---|
| Stories about specific past experiences ("Last Tuesday I…") | Generic opinions ("I usually…" / "I would…") |
| What the user *actually does*, not what they think they should do | Hypothetical feature requests ("It would be nice if…") |
| Moments of visible frustration, confusion, or workaround | Guiding towards solutions the team already has in mind |
| Emotional language that signals pain or delight | Yes/no questions that close down storytelling |

**In real life:** A skilled interviewer also watches for *non-verbal cues* — hesitations, sighs, eye-rolls, or the energy shift when a topic is sensitive. These body-language signals often reveal more than words. You cannot observe these cues in a text interview, so train yourself to probe deeper whenever an answer feels thin: *"Can you tell me more about that?"* or *"What happened next?"*

**In this training:** Because we cannot access real users during a 1-day session, the **DesignSprintAgent will simulate a realistic user** based on your Product Brief. The agent will stay in character throughout the interview, responding as that user would — with plausible frustrations, habits, and language. This lets you practice interview technique and still extract meaningful, contextually grounded insights to carry forward.

---

## How DesignSprintAgent Runs This Activity

The agent runs in two distinct modes during this activity:

- **Facilitator mode** (before and after the interview): guides setup, debrief, and insight synthesis.
- **User mode** (during the interview): the agent speaks *as the simulated user*. It will not break character unless the interviewer asks for help, at which point it will briefly step out and offer a suggested question, marked with `[HINT]`, then return to character.

The interview is time-boxed to **10–15 minutes**. The agent will signal when time is running short. After the interview, the agent exits character and synthesises the conversation into pain points, opportunities, quotes, and HMW suggestions.

At the end, the agent will offer to run an **additional round** with a different user type if the group wants more perspectives.

**To start, say:** `@DesignSprintAgent let's run User Interviews`

---

## Step 1 — Orientation

**What the agent does:** Explains the purpose and ground rules of the activity to the group, including the Copilot simulation approach and what good interviewing looks like. Confirms the group is ready before moving to persona preparation.

> **Agent prompt to group:**
> *"Welcome to User Interviews. Here's what we're doing and why:*
>
> *The goal of a User Interview is to surface real pain points and opportunities from the user's perspective — not to validate solutions you already have in mind. You're here to listen and learn, not to pitch or explain.*
>
> *Because we're in a 1-day training and can't access real users right now, I'll be simulating a realistic user for you based on the Product Brief. I'll stay in character throughout the interview and respond as that user would — with real frustrations, habits, and language.*
>
> *If you get stuck and don't know what to ask next, just type `help` and I'll suggest a question without breaking the flow for too long.*
>
> *The interview will run for 10–15 minutes. Your job is to ask open questions, follow stories, and listen for pain. Ready? Reply `ready` and we'll prepare your user."*

---

## Step 2 — Prepare the Simulated User

**What the agent does:** Reads the Product Brief from `design-sprint/phase-1-understand/product-brief.md`. Based on the target users, core problem, and context described there, proposes a specific simulated user profile: name, role, organisation type, relevant background, likely pain points, and likely opportunities. Presents the profile to the group for confirmation or adjustment before the interview begins.

> **Agent prompt to group:**
> *"Based on your Product Brief, here is the user I'm going to simulate for this interview:*
>
> *[Agent presents the proposed user profile here — see Simulated User Profile table below]*
>
> *Does this feel like a realistic and useful person to interview for your sprint? If you'd like to adjust the role, context, or type of problems this user faces, tell me now. Otherwise reply `confirmed` and we'll begin the interview."*

## Simulated User Profile

| Field | Value |
|---|---|
| Name (fictional) | _(DesignSprintAgent fills in — e.g. "Sarah")_ |
| Role / Job Title | _(DesignSprintAgent fills in — derived from Product Brief target users)_ |
| Organisation Type | _(DesignSprintAgent fills in — e.g. "Mid-sized logistics company, ~200 employees")_ |
| Experience Level | _(DesignSprintAgent fills in — e.g. "5 years in this role, not very technical")_ |
| Current Relevant Behaviour | _(DesignSprintAgent fills in — what this user currently does related to the problem space)_ |
| Likely Pain Points | _(DesignSprintAgent fills in — 2–3 plausible frustrations grounded in the Product Brief)_ |
| Likely Opportunities | _(DesignSprintAgent fills in — 1–2 areas where this user would most benefit from improvement)_ |

---

## Step 3 — Live Interview

**What the agent does:** Switches into **User mode** and greets the interviewer in character as the simulated user. Responds naturally to questions, sharing experiences, frustrations, and workarounds as that user would. Does not volunteer pain points unprompted — the interviewer must ask. If the interviewer types `help`, the agent briefly steps out of character, offers a `[HINT]` question suggestion, then returns to character. Signals at the 12-minute mark if the time limit is approaching.

> **Agent prompt to group (in character):**
> *"[Agent greets the interviewer as the simulated user, introducing themselves naturally — e.g. "Hi, I'm Sarah. Thanks for making time to chat — happy to talk about how things are going in my day-to-day."]"*

**Hints the agent may offer if the interviewer types `help`:**

The agent will suggest context-appropriate questions based on where the conversation is. General examples of hint patterns:

- `[HINT] Try asking: "Can you walk me through the last time you had to deal with [topic]? What happened?"`
- `[HINT] Try asking: "What's the most frustrating part of that process for you?"`
- `[HINT] Try asking: "What do you do when that goes wrong? How do you work around it?"`
- `[HINT] Try asking: "How does that affect you — or the people you work with?"`
- `[HINT] Try asking: "If that problem went away tomorrow, what would be different for you?"`

> *(The agent records the full interview conversation here as it happens, in a simple transcript format: **Interviewer:** … / **[User name]:** …)*

## Interview Transcript

> *(DesignSprintAgent records the live interview exchange here as it unfolds)*

| Speaker | Message |
|---|---|
| _(DesignSprintAgent fills in progressively)_ | _(DesignSprintAgent fills in progressively)_ |

---

## Step 4 — Debrief: Extract Pain Points

**What the agent does:** Exits User mode and returns to Facilitator mode. Analyses the interview transcript and identifies concrete frustrations, blockers, and unmet needs expressed by the simulated user. Presents each with a supporting quote, then asks the group to confirm or add to the list.

> **Agent prompt to group:**
> *"Great interview. Let me step out of character now and help you debrief.*
>
> *Here are the key pain points I identified from our conversation — things the user explicitly or implicitly told us were frustrating, broken, or hard. Review the list, then reply `confirmed` or suggest any changes."*

## Key Pain Points

| # | Pain Point | Supporting Quote from Interview |
|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in from transcript analysis)_ | _(DesignSprintAgent fills in — verbatim from the interview)_ |
| | | |

---

## Step 5 — Debrief: Identify Opportunities

**What the agent does:** From the pain points and the shape of the conversation, names the areas where a design or process change could deliver meaningful value. Frames each as an opportunity (what could be better) rather than a solution (how to fix it). Confirms with the group.

> **Agent prompt to group:**
> *"Based on the pain points, here are the opportunity areas — places where something better could make a real difference for this user. These are not solutions yet; they're directions worth exploring. Reply `confirmed` or suggest adjustments."*

## Opportunities Identified

| # | Opportunity Area | Connection to Pain Point |
|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in from transcript analysis)_ | _(DesignSprintAgent fills in — e.g. "Addresses pain point #2")_ |
| | | |

---

## Step 6 — Capture Notable Quotes

**What the agent does:** Selects 2–4 quotes from the interview that most vividly capture the user's frustration, mental model, or emotional state. These are used as evidence in Phase 2 when crafting the Problem Statement.

> **Agent prompt to group:**
> *"Here are the quotes from the interview I'd carry forward — the ones that most authentically capture what this user experiences. These will ground the Problem Statement in Phase 2. Confirm or swap any you'd prefer. Reply `confirmed` or share alternatives."*

## Notable Quotes

> _(DesignSprintAgent fills in — Quote 1, verbatim from the interview transcript)_

> _(DesignSprintAgent fills in — Quote 2, verbatim from the interview transcript)_

> _(DesignSprintAgent fills in — Quote 3, if available)_

> _(DesignSprintAgent fills in — Quote 4, if available)_

---

## Step 7 — Generate "How Might We" Suggestions

**What the agent does:** Generates 3–5 HMW questions derived directly from the pain points and opportunities surfaced in this interview. These seed the optional HMW Notes activity in Phase 1 and the HMW Clustering in Phase 2.

> **Agent prompt to group:**
> *"Finally, here are 'How Might We' questions generated from this interview — seeds for deeper brainstorming later. Review and confirm, or suggest improvements. Reply `confirmed` or share your own alternatives."*

## "How Might We" Suggestions

| # | HMW Question | Derived From |
|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in — e.g. "How might we…?")_ | _(DesignSprintAgent fills in — e.g. "Pain point #2 + opportunity #1")_ |
| | | |

---

## Step 8 — Offer Additional Interview Round

**What the agent does:** Asks the group whether they would like to run another interview round with a different type of user. If yes, proposes a contrasting user profile — a different role, experience level, or relationship to the problem — and repeats Steps 2–7. Each additional round is saved as a separate artefact file.

> **Agent prompt to group:**
> *"That's one interview done. Getting insights from just one user type can leave blind spots — different users experience the same product in very different ways.*
>
> *Would you like to run a second interview with a different type of user? If yes, I'll suggest a contrasting profile based on your Product Brief (e.g. a less experienced user, a user in a different role, or someone who uses the product in a different context). Reply `yes` for another round or `done` to close this activity."*

| Follow-up Round | Simulated User Type | Completed |
|---|---|---|
| Round 1 | _(DesignSprintAgent fills in — from Step 2)_ | _(✅ Done)_ |
| Round 2 | _(DesignSprintAgent fills in if requested)_ | _(⬜ Pending / ✅ Done)_ |
| Round 3 | _(DesignSprintAgent fills in if requested)_ | _(⬜ Pending / ✅ Done)_ |

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to HMW Notes and User Journey Mapping.)*

| Field | Value |
|---|---|
| Simulated User Profile(s) | _(DesignSprintAgent fills in — role and key context for each round)_ |
| Top Pain Point | _(DesignSprintAgent fills in — the single most important frustration surfaced)_ |
| Top Opportunity | _(DesignSprintAgent fills in — the highest-potential area for design intervention)_ |
| Total Pain Points Identified | _(DesignSprintAgent fills in)_ |
| Total HMW Suggestions Generated | _(DesignSprintAgent fills in)_ |
| Interview Rounds Completed | _(DesignSprintAgent fills in)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important reframe or discovery from the full session)_ |

### Feed-forward to HMW Notes and User Journey Map

| Downstream Artefact | How this activity informs it |
|---|---|
| **HMW Notes** | The HMW suggestions generated in Step 7 seed the full HMW brainstorm; pain points provide the raw material for additional reframes |
| **User Journey Map** | Pain points and opportunity areas reveal which steps in the user journey to focus on and where emotions are most negative |
| **Problem Statement (Phase 2)** | Notable quotes provide the evidence layer; the top pain point and opportunity become the core of the Problem Statement |
| **User Persona (Phase 2)** | The simulated user profile, behaviour patterns, and mental models feed directly into the Persona's goals, frustrations, and context |

> **Suggested first HMW brainstorm prompt** *(generated by DesignSprintAgent from the top pain point)*:
>
> _(DesignSprintAgent generates a suggested HMW reframe here, e.g. "How might we help [user type] [achieve goal] without [current blocker]?")_

---

## Notes & Observations

> *(Patterns across interview rounds, questions the interviewer struggled to ask, moments where the simulated user's responses surprised the group, alternative user types worth exploring in a real sprint.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take the pain points and HMW suggestions into the **"How Might We" Notes** activity or the **User Journey Map**.
> Invoke `@DesignSprintAgent let's run How Might We Notes` or `@DesignSprintAgent let's run User Journey Map` to continue Phase 1.
