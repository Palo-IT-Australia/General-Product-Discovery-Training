---
description: "Use when adding a new Design Sprint activity template to any phase of the design-sprint/ workspace. Covers the required file structure, section patterns, agent facilitation conventions, DesignSprintAgent registration, and feed-forward linkage to downstream artefacts. Use this whenever a new activity template file needs to be created, or when reviewing whether an existing template follows the correct pattern."
---

# Design Sprint Activity Template — Authoring Pattern

Every activity template in this workspace is a **live facilitation document**: the DesignSprintAgent reads it to understand how to run the activity, fills it in progressively during a session by collecting group input via Copilot Chat, and produces a completed artefact at the end. Static worksheets are not acceptable — every template must follow the interactive pattern below.

---

## 1. File Location

```
design-sprint/phase-{N}-{phase-name}/templates/{activity-slug}.md
```

| Phase | Folder |
|---|---|
| Phase 1 — Understand | `design-sprint/phase-1-understand/templates/` |
| Phase 2 — Define | `design-sprint/phase-2-define/templates/` |
| Phase 3 — Sketch | `design-sprint/phase-3-sketch/templates/` |
| Phase 4 — Decide | `design-sprint/phase-4-decide/templates/` |

Use kebab-case for the filename (e.g. `business-question-to-human-question.md`).

---

## 2. Required Sections (in order)

### 2.1 Agent Header *(first line of document)*

```markdown
> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides the group through each step, collects input via Copilot Chat, and populates this document progressively. Do not edit manually during a live session.
```

This must always be the very first line. It acts as the ownership marker that tells Copilot this is an agent-owned artefact.

---

### 2.2 Metadata Line

A single line immediately after the header providing at-a-glance activity facts:

```markdown
**Activity type:** {Group | Individual | Pair} | **Time:** {N} minutes | **Sprint phase:** Phase {N} — {Phase Name}
**Source:** [{Author/Organisation}]({source-url}) via [Google Design Sprint Kit]({dsk-url})
```

If there is no external source, omit the Source line.

---

### 2.3 Session Details Table

```markdown
## Session Details

| Field | Value |
|---|---|
| Date | _(DesignSprintAgent fills in)_ |
| Participants | _(DesignSprintAgent fills in from introductions)_ |
| Sprint Context | _(DesignSprintAgent fills in from sprint tracker)_ |
| Facilitator | DesignSprintAgent |
```

The agent populates this at the start of every session. Do not pre-fill any values.

---

### 2.4 About This Activity

Explain the purpose of the activity in plain language. Include:

- A 1–2 sentence **purpose statement** explaining what the activity achieves and why it matters in its phase
- A **comparison or concept table** where the activity involves distinguishing between two things (e.g., business vs human questions, pain points vs opportunities)
- A **worked example** using *italics* to show the before/after or input/output of the activity

```markdown
## About This Activity

{Purpose statement — what the activity achieves and why it matters at this phase.}

| Concept A | Concept B |
|---|---|
| {characteristic} | {characteristic} |

**Example:**
{Input}: *"{example input}"*
→ {Output}: *"{example output}"*
```

If the activity does not involve a contrast, omit the table and just use the purpose statement and example.

---

### 2.5 How DesignSprintAgent Runs This Activity

This section explains the agent's facilitation loop and provides the trigger phrase the group uses to start.

```markdown
## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run {Activity Name}`
```

The trigger phrase must exactly match the activity name used in the DesignSprintAgent's activity list (see Section 4).

---

### 2.6 Steps

Each step in the activity gets its own `## Step N — {Step Name}` section containing **three elements**:

#### Element A: What the agent does

A short sentence describing the agent's role at this step (not the participant's role):

```markdown
**What the agent does:** {Description of agent behaviour — e.g. "Time-boxes 5 minutes of individual brainstorm, prompts each participant to contribute, then records all responses."}
```

#### Element B: Agent prompt to group

The exact words the agent says to the group, formatted as a blockquote. This must include:
- Clear instructions on what participants should do
- The **expected reply format** so the agent can parse responses (e.g., `[Your name]: How do people…?`)
- Any time constraints

```markdown
> **Agent prompt to group:**
> *"{Exact facilitation text the agent delivers. Include expected reply format in backticks if applicable.}"*
```

#### Element C: Output placeholder

A table or blockquote that the agent fills in during the session. Use `_(DesignSprintAgent fills in...)_` as the placeholder value — never leave cells truly empty, as empty cells cause confusion about intent.

```markdown
| Column A | Column B |
|---|---|
| _(name)_ | _(DesignSprintAgent populates from chat responses)_ |
| | |
```

For single-value outputs (e.g., a committed question), use a blockquote:

```markdown
> _(DesignSprintAgent records {the output} here once the group confirms)_
```

---

### 2.7 Session Summary

The closing output table, populated by the agent at the end of the session. It must capture the most important outputs in a scannable format, and include a **Key Insight** field — the single most important reframe or discovery from the session.

```markdown
## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to subsequent activities.)*

| Field | Value |
|---|---|
| {Primary input label} | _(DesignSprintAgent fills in)_ |
| {Primary output label} | _(DesignSprintAgent fills in)_ |
| {Runner-up or alternatives label} | _(DesignSprintAgent fills in)_ |
| Total {items} Generated | _(DesignSprintAgent fills in)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important {reframe/discovery/decision} that emerged)_ |
```

---

### 2.8 Feed-forward Section

Every template must explicitly connect this activity's outputs to the **next downstream artefact** in the sprint. This ensures the DesignSprintAgent knows exactly what to do with the session output after the activity closes.

```markdown
### Feed-forward to {Downstream Artefact Name}

The {output of this activity} directly shapes how the {downstream artefact} is constructed:

| {Downstream Artefact} Field | How this activity informs it |
|---|---|
| **{Field name}** | {One sentence on how the output maps to this field} |
| **{Field name}** | {One sentence} |
| **{Field name}** | {One sentence} |

> **Suggested {downstream artefact} {field}** *(generated by DesignSprintAgent from the {primary output})*:
>
> _(DesignSprintAgent generates a suggested {field value} here, e.g. "{example suggestion pattern}")_
```

Common downstream artefacts by phase:

| Current Activity Phase | Typical Feed-forward Target |
|---|---|
| Phase 1 — Understand | User Journey Map, HMW Notes |
| Phase 2 — Define | Problem Statement, Sprint Questions, User Persona |
| Phase 3 — Sketch | Solution Sketch, Silent Review notes |
| Phase 4 — Decide | Storyboard |

---

### 2.9 Notes & Observations

```markdown
## Notes & Observations

> *(Any tensions surfaced during the session, alternative options worth revisiting, dissenting views, or follow-up actions the group identified.)*

_(DesignSprintAgent records observations from the chat discussion here)_
```

---

### 2.10 Closing Next Step Callout *(last line of document)*

```markdown
> **Next Step:** Take the {primary output} and Session Summary into the **{Next Activity Name}** activity.
> Invoke `@DesignSprintAgent {trigger phrase for next activity}` to continue Phase {N}.
```

---

## 3. Full Skeleton

Use this as a starting point when creating a new template from scratch:

```markdown
> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides the group through each step, collects input via Copilot Chat, and populates this document progressively. Do not edit manually during a live session.

**Activity type:** {Group | Individual | Pair} | **Time:** {N} minutes | **Sprint phase:** Phase {N} — {Phase Name}
**Source:** [{Author}]({url}) via [Google Design Sprint Kit]({dsk-url})

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

{Purpose statement.}

| Concept A | Concept B |
|---|---|
| {characteristic} | {characteristic} |

**Example:**
{Input}: *"{example}"*
→ {Output}: *"{example}"*

---

## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run {Activity Name}`

---

## Step 1 — {Step Name}

**What the agent does:** {Agent behaviour description.}

> **Agent prompt to group:**
> *"{Exact facilitation text. Reply format: `[Your name]: {expected format}`}"*

| {Column A} | {Column B} |
|---|---|
| _(name)_ | _(DesignSprintAgent populates from chat responses)_ |
| | |

---

## Step 2 — {Step Name}

**What the agent does:** {Agent behaviour description.}

> **Agent prompt to group:**
> *"{Exact facilitation text.}"*

| {Column A} | {Column B} |
|---|---|
| _(DesignSprintAgent fills in)_ | |

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity.)*

| Field | Value |
|---|---|
| {Primary input} | _(DesignSprintAgent fills in)_ |
| {Primary output} | _(DesignSprintAgent fills in)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in)_ |

### Feed-forward to {Downstream Artefact}

| {Downstream Artefact} Field | How this activity informs it |
|---|---|
| **{Field}** | {One sentence} |

> **Suggested {field}** *(generated by DesignSprintAgent)*:
>
> _(DesignSprintAgent generates a suggestion here)_

---

## Notes & Observations

> *(Tensions surfaced, alternatives worth revisiting, dissenting views, follow-up actions.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take the {output} into the **{Next Activity}** activity.
> Invoke `@DesignSprintAgent {trigger phrase}` to continue Phase {N}.
```

---

## 4. After Creating the Template — Required Follow-up Steps

Creating the template file alone is not enough. Complete both of the following:

### 4.1 Register the activity in DesignSprintAgent

Open `.github/agents/DesignSprintAgent.md` and add the new activity to the correct phase list under **"Activity Suggestions"** (Section 2 of the agent's Core Responsibilities). Follow the existing bullet format:

```markdown
- **{Activity Name}**: {One sentence describing what it achieves and when to use it.}
```

Also add a processing workflow block under **"Information Processing & Artefact Storage"** (Section 4) if the activity produces an artefact that the agent needs to save. Follow the lettered subsection pattern (A, B, C…) already used there.

### 4.2 Register the activity in the Sprint Tracker

Open `design-sprint/sprint-tracker.md` and add a row to the correct phase table:

```markdown
| {Activity Name} | ⬜ Pending | `phase-{N}-{name}/{activity-slug}.md` | — |
```

---

## 5. Quality Checklist

Before finishing, verify:

- [ ] File is in the correct `templates/` folder for its phase
- [ ] First line is the `> **Facilitated by DesignSprintAgent.**` header (exact wording)
- [ ] Trigger phrase in "How DesignSprintAgent Runs This Activity" matches the activity name used in `.github/agents/DesignSprintAgent.md`
- [ ] Every step has all three elements: "What the agent does", "Agent prompt to group", output placeholder
- [ ] Every output placeholder uses `_(DesignSprintAgent fills in...)_` — no truly empty cells
- [ ] Session Summary table includes a "Key Insight Surfaced" row
- [ ] Feed-forward section explicitly names the downstream artefact and maps at least 3 fields
- [ ] Closing "Next Step" callout includes the trigger phrase for the next activity
- [ ] Activity registered in `.github/agents/DesignSprintAgent.md`
- [ ] Activity registered in `design-sprint/sprint-tracker.md`
