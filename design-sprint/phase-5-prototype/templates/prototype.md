> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides the group through each step, collects input via Copilot Chat, and populates this document progressively. Do not edit manually during a live session.

**Activity type:** Group | **Time:** 60–120 minutes | **Sprint phase:** Phase 5 — Prototype
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

Prototyping transforms the Prototype Slice — the prioritised set of user stories identified during Story Mapping — into a tangible, testable artefact. The goal is not to build a finished product, but to create the minimum experience needed to validate the Problem Statement with real users.

> **Training Note:** In this 1-day training, GitHub Copilot can directly assist with building **digital prototypes** (web/mobile interfaces, APIs, scripts, data dashboards, chatbot flows). For this session, the agent will identify which stories in your Prototype Slice are digital in nature and prioritise those for Copilot-assisted development — even if they rank lower in RICE score than non-digital items. This is intentional: the purpose of today's training is to experience how Copilot accelerates product prototyping.
>
> Non-digital stories (physical products, printed materials, service blueprints, offline workflows) are equally important and must be prototyped outside of Copilot. If your Prototype Slice contains non-digital stories, the agent will provide specific guidance on how to prototype and validate them independently of this session.
>
> If your entire Prototype Slice is non-digital, the agent will guide you through offline prototyping approaches and validation techniques so you still walk away with a clear plan.

| Digital Prototype (Copilot-assisted) | Non-Digital Prototype (Outside Copilot) |
|---|---|
| Web or mobile UI (HTML, React, etc.) | Physical product mockup |
| API or backend feature | Service blueprint / role-play scenario |
| Data dashboard or report | Printed worksheet or paper prototype |
| Notification or messaging flow | Offline workflow or process diagram |
| Chatbot or conversational interface | In-person facilitated experience |

**Example:**
Prototype Slice: *"Show AI-suggested reply before sending (RICE: 6.4) + Print confirmation slip at counter (RICE: 8.1)"*
→ Agent offers: *"'Show AI-suggested reply' is digital — let's build this with Copilot first, even though it has a lower RICE score. 'Print confirmation slip' is non-digital — I'll give you a step-by-step plan to prototype that outside of Copilot."*

---

## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run Prototype`

---

## Step 1 — Load Prototype Slice

**What the agent does:** Reads `design-sprint/phase-4-decide/story-mapping.md` and extracts all stories marked as the Prototype Slice. Presents them to the group for confirmation before any prototyping begins.

> **Agent prompt to group:**
> *"Let me load the Prototype Slice from our Story Mapping session. Here are the stories the group agreed to prototype, in RICE priority order. Review the list and confirm it still reflects your intent — if anything has changed, tell me now. Reply `confirmed` or describe any updates."*

| # | User Story | RICE Score | Slice Status |
|---|---|---|---|
| _(DesignSprintAgent fills in from story-mapping.md)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(In Prototype Slice / Not in Slice)_ |
| | | | |

---

## Step 2 — Classify Stories: Digital vs Non-Digital

**What the agent does:** Analyses each story in the Prototype Slice and classifies it as Digital (GitHub Copilot can help build it) or Non-Digital (prototyping must happen outside Copilot). Presents the classification with a brief rationale for each story, then asks the group to confirm or correct it.

> **Agent prompt to group:**
> *"I've classified each story in the Prototype Slice as Digital or Non-Digital. Digital stories are ones where Copilot can scaffold the code, UI, or logic. Non-digital stories need to be prototyped using physical materials, role-play, printed forms, or other offline methods.*
>
> *Review my classification and let me know if you disagree with any item. Reply `confirmed` or tell me which stories to reclassify and why."*

> **Training reminder:** For this session, **digital stories will be prototyped first using GitHub Copilot** regardless of their RICE rank relative to non-digital stories. Non-digital stories are equally important in a real sprint — plan to complete those outside of today's session using the guidance in Step 5.

| # | User Story | RICE Score | Classification | Reasoning |
|---|---|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(Digital / Non-Digital)_ | _(DesignSprintAgent fills in — e.g. "UI feature — can be scaffolded in HTML/React with Copilot")_ |
| | | | | |

---

## Step 3 — Confirm Build Order

**What the agent does:** Defines the session build sequence — digital stories first (sorted by RICE score), then non-digital stories (listed for offline follow-up). Presents the ordered plan and gets group sign-off before proceeding to the build.

> **Agent prompt to group:**
> *"Here is the build order for today's session. Digital stories come first so we can prototype them together with Copilot. Non-digital stories are listed after — I'll give you a detailed offline plan for those in Step 5. Confirm the order or tell me of any changes. Reply `confirmed` or describe any adjustments."*

| Build # | User Story | Type | Planned Approach |
|---|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(Digital / Non-Digital)_ | _(DesignSprintAgent fills in — e.g. "React component via Copilot" / "Paper prototype — see Step 5 for guidance")_ |
| | | | |

---

## Step 4 — Build Digital Prototype with Copilot

**What the agent does:** Guides the group through building each digital story one at a time using GitHub Copilot. For each story, generates a tailored Copilot prompt the group can use as a starting point, then records what was built and the output file path. If there are no digital stories, skips this step and notes it.

> **Agent prompt to group:**
> *"Let's build the digital stories one at a time. For each story, I'll give you a suggested Copilot prompt to get started. Paste it into Copilot Chat, iterate from there, and tell me when you're satisfied with the output. Reply `done: [story name]` once each story is complete and tell me the file path of anything saved."*

> *(If there are no digital stories in the Prototype Slice, the agent will record: "No digital stories identified in the Prototype Slice — Step 4 skipped. Proceeding to non-digital guidance in Step 5.")*

| # | User Story | Suggested Copilot Prompt | Output / File Created | Status |
|---|---|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in)_ | _(DesignSprintAgent generates a tailored Copilot prompt for this specific story)_ | _(DesignSprintAgent fills in once the group confirms the build is done)_ | _(⬜ Pending / ✅ Done)_ |
| | | | | |

---

## Step 5 — Plan Non-Digital Prototypes

**What the agent does:** For each non-digital story, provides a specific prototype method, guidance on what to focus on during the prototype session, and instructions on how to validate it with users. If all stories are digital, records that this step is not needed.

> **Agent prompt to group:**
> *"For the non-digital stories in your Prototype Slice, here is a specific plan for how to prototype and validate each one outside of Copilot. These prototypes are just as important as the digital ones for validating your Problem Statement — make sure to schedule time after this session to complete them.*
>
> *Review the plan, ask questions, then reply `understood` to close the session."*

> *(If all Prototype Slice stories are digital, the agent will record: "All Prototype Slice stories are digital — no non-digital prototype plan required for this session.")*

| # | User Story | Prototype Method | What to Build / Simulate | What to Focus On | How to Validate |
|---|---|---|---|---|---|
| _(DesignSprintAgent fills in)_ | _(DesignSprintAgent fills in — e.g. "Paper prototype", "Role-play script", "Printed form", "Service blueprint")_ | _(DesignSprintAgent fills in — e.g. "Draw the key screen on paper, with a facilitator acting as the system and turning pages to simulate responses")_ | _(DesignSprintAgent fills in — e.g. "The information hierarchy and the primary call-to-action")_ | _(DesignSprintAgent fills in — e.g. "Can the user complete the task without prompting? Do they understand what action to take next?")_ | _(DesignSprintAgent fills in — e.g. "Run a 10-minute observation with 2–3 real users; note every hesitation or spoken confusion without intervening")_ |
| | | | | | |

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to User Testing.)*

| Field | Value |
|---|---|
| Total Stories in Prototype Slice | _(DesignSprintAgent fills in)_ |
| Digital Stories Built with Copilot | _(DesignSprintAgent fills in)_ |
| Non-Digital Stories Planned | _(DesignSprintAgent fills in)_ |
| Prototype Files Created | _(DesignSprintAgent fills in — list of relative file paths for all digital outputs)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important discovery or constraint that emerged during the build)_ |

### Feed-forward to User Testing

The prototype(s) and validation plan produced here directly shape how user testing is structured:

| User Testing Field | How this activity informs it |
|---|---|
| **Test Scenarios** | Each Prototype Slice story becomes a task scenario for the user test — one task per story |
| **Success Criteria** | The "What to Focus On" and "How to Validate" columns define what success looks like for each task |
| **Prototype Materials** | Digital prototype files and non-digital materials are handed to the test facilitator before sessions begin |
| **Test Priority Order** | RICE scores determine which scenarios to run first if session time is limited |
| **Hypotheses to Test** | The Problem Statement guides the overarching hypothesis: does this prototype validate or invalidate our assumption? |

> **Suggested first user test scenario** *(generated by DesignSprintAgent from the top-priority Prototype Slice story)*:
>
> _(DesignSprintAgent generates a suggested scenario here, e.g. "Ask the user to [perform the key action] using the prototype and observe whether they can [achieve the goal] without any prompting or explanation from the facilitator.")_

---

## Notes & Observations

> *(Tensions surfaced during the build, design decisions made, alternatives worth revisiting, follow-up actions.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take the prototype files and non-digital prototype plan into **User Testing**.
> Invite real users to test the prototype and observe their behaviour against the success criteria defined above.
