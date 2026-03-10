# Business Question to Human Question

> **Facilitated by DesignSprintAgent.** Invoke `@DesignSprintAgent` to run this activity interactively. The agent guides the group through each step, collects input via Copilot Chat, and populates this document progressively. Do not edit manually during a live session.

**Activity type:** Group | **Time:** 20 minutes | **Sprint phase:** Phase 1 — Understand  
**Source:** [Sudden Compass®](https://suddencompass.com/) via [Google Design Sprint Kit](https://designsprintkit.withgoogle.com/methodology/phase1-understand/business-question-human-question)

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

Business Question to Human Question (by Sudden Compass®) helps teams break out of company-centric thinking by reframing a business goal as a customer-centred question — uncovering new opportunities to genuinely meet customer needs.

| Business Question | Human Question |
|---|---|
| Aimed at a financial or operational outcome | Aimed at understanding customer behaviours and needs |
| Centred on company goals or metrics | No reference to company goals or metrics |
| Often uses internal jargon | Understandable to a general audience |

**Example:**  
Business question: *"How do we drive more top-tier subscriptions to our music streaming service?"*  
→ Human questions: *"How do people listen to music?"* / *"What value do people derive from listening to music?"*

---

## How DesignSprintAgent Runs This Activity

The agent executes the following sequence in Copilot Chat. At each step it will:

1. **Prompt** — present a facilitating question or instruction to the group
2. **Collect** — ask participants to share their input directly in chat
3. **Record** — populate the relevant section of this document with the group's responses
4. **Confirm** — check the group is ready, then advance to the next step

**To start, say:** `@DesignSprintAgent let's run Business Question to Human Question`

---

## Step 1 — Align on the Business Question

**What the agent does:** Opens the activity, explains the purpose, and asks the group to agree on a single business question.

> **Agent prompt to group:**
> *"Let's start by agreeing on the business question that is driving this sprint. What is the key business challenge or goal your team is focused on right now? Try to frame it as: 'How do we [achieve business outcome]?' — for example: 'How do we increase sales conversions in Q1?' Share your suggestion in chat, then we'll align as a group."*

**Business Question agreed by the group:**

> _(DesignSprintAgent records the agreed business question here once the group confirms alignment)_

---

## Step 2 — Generate Human Questions *(5 mins, individual)*

**What the agent does:** Time-boxes 5 minutes of individual brainstorm, prompts each participant to contribute, then records all responses. If any participant is unsure where to start, the agent reviews the agreed business question and generates a set of example human questions to spark thinking — clearly labelling them as suggestions, not answers.

> **Agent prompt to group:**
> *"Now let's look at this from our customers' perspective. Individually, take 5 minutes to write as many human questions as you can. Human questions should:*
> - *Focus on understanding people's behaviours, needs, or motivations*
> - *Contain no company goals, metrics, or jargon*
> - *Be understandable to anyone outside your company*
>
> *Share each question as a separate message in this format: `[Your name]: How do people…?`*
> *I'll collect everything as you go. Start now — you have 5 minutes!*
>
> *Not sure where to start? Just reply `suggest` and I'll offer a few example human questions based on your business question to help get you thinking — they're only a starting point, so feel free to go in a completely different direction."*

**Agent behaviour when a participant replies `suggest`:**

The agent re-reads the agreed business question from Step 1 and generates 3–5 example human questions using the following logic:
- Strip out any reference to company goals, metrics, products, or financial outcomes
- Identify the underlying human behaviour or need implied by the business question
- Reframe it as open-ended questions about how people think, feel, or act

The agent presents them as stimulus only:

> *"Here are a few example human questions to spark your thinking — these are just starting points, not the 'right' answers:*
> - *[Generated question 1]*
> - *[Generated question 2]*
> - *[Generated question 3]*
>
> *Use these as inspiration, challenge them, or ignore them entirely. What questions come to mind for you?"*

| Participant | Human Questions Generated |
|---|---|
| _(name)_ | _(DesignSprintAgent populates from chat responses)_ |
| | |
| | |
| | |
| | |

---

## Step 3 — Share, Read Aloud & Cluster

**What the agent does:** Presents the full list of human questions back to the group, facilitates a discussion to identify themes, and clusters questions accordingly. If the group is unsure how to form clusters, the agent proposes an initial grouping based on the questions collected and invites the group to adjust it.

> **Agent prompt to group:**
> *"Great work — here are all the human questions we've generated [agent displays the table above]. Let's cluster similar ones together. Looking at this list, what themes or groupings do you see? Name each cluster and tell me which questions belong to it. I'll organise them as you discuss.*
>
> *Not sure how to cluster them? Reply `suggest clusters` and I'll propose an initial grouping for you to react to."*

**Agent behaviour when the group replies `suggest clusters`:**

The agent reviews all collected human questions and proposes themes by identifying shared subjects, verbs, or underlying concerns:

> *"Here's a suggested clustering to react to — move questions between groups or rename themes as you see fit:*
>
> **[Suggested theme 1]:** [Question A], [Question B]*
> **[Suggested theme 2]:** [Question C], [Question D]*
>
> *Does this feel right, or would you organise them differently?"*

| Cluster / Theme | Human Questions in this cluster |
|---|---|
| _(theme name)_ | _(DesignSprintAgent populates based on group discussion)_ |
| | |
| | |
| | |

---

## Step 4 — Prioritise *(Dot Voting)*

**What the agent does:** Explains how dot voting works and instructs the group to vote physically using sticky dots, markers, or a show of hands. Once the physical vote is complete, the agent asks for the tally to be reported back, then ranks the results. If a participant is unsure which questions deserve their votes before the physical vote, the agent offers a short evaluation against a novelty and customer-centricity lens to help them decide.

> **Agent prompt to group:**
> *"Time to vote! Here's how dot voting works:*
>
> - *Each person gets **3 dot votes** — use sticky dots, marker ticks, or a show of hands*
> - *Place your votes on the human questions you believe are most likely to uncover something genuinely new and unknown about your customers*
> - *You can spread your votes across different questions, or stack them all on one if you feel strongly about it*
>
> *Go ahead and vote physically now. When everyone has voted, count up the dots on each question and report the results back to me in this format:*
> `[Total votes] for [Question]`
> *(one line per question, e.g. `3 for "How do people decide when to buy a car?"`)*
>
> *Unsure which questions to vote for? Reply `help me choose` before you vote and I'll share a quick take on which questions seem most likely to surface genuinely new customer insight."*

**Agent behaviour when a participant replies `help me choose`:**

The agent reviews the clustered questions and evaluates each against two criteria — **novelty** (how likely the question is to reveal something not already known) and **customer centricity** (how far removed it is from the business question). It presents a brief, non-prescriptive evaluation to inform — not replace — the physical vote:

> *"Here's a quick take to inform your own judgement — the final call is yours:*
>
> - *[Question A] — [one sentence on why it might surface new insight]*
> - *[Question B] — [one sentence]*
> - *[Question C] — [one sentence on why it may be too close to the original business question]*
>
> *I'd lean towards [Question A] and [Question B] as strong candidates for uncovering something new, but vote with your gut — what feels most unexplored to you?"*

| Rank | Human Question | Votes |
|---|---|---|
| 1 | _(DesignSprintAgent fills in after tally)_ | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |

---

## Step 5 — Commit to a Single Human Question

**What the agent does:** Presents the top-voted question, invites the group to confirm or discuss, then records the final committed question with the group's rationale.

> **Agent prompt to group:**
> *"Based on the votes, your top human question is: **[top-ranked question]**. Does the group agree to commit to this as the human question guiding this sprint? Reply 'agreed' to lock it in, or share your thoughts if you'd like to discuss further before deciding."*

**Chosen Human Question:**

> _(DesignSprintAgent records the committed human question here once the group confirms)_

**Rationale** *(why the group chose this question)*:

> _(DesignSprintAgent summarises the group's reasoning from the chat discussion)_

---

## Session Summary

> *(Populated by DesignSprintAgent at the close of the activity. This is the output handed forward to subsequent activities.)*

| Field | Value |
|---|---|
| Business Question | _(DesignSprintAgent fills in)_ |
| Chosen Human Question | _(DesignSprintAgent fills in)_ |
| Runner-Up Questions | _(DesignSprintAgent fills in top 2–3 alternatives)_ |
| Total Human Questions Generated | _(DesignSprintAgent fills in)_ |
| Key Insight Surfaced | _(DesignSprintAgent fills in — the most important reframe that emerged)_ |

### Feed-forward to User Journey Map

The chosen human question directly shapes how the User Journey Map is constructed:

| User Journey Map Field | How this activity informs it |
|---|---|
| **Scenario** | The chosen human question defines the scenario to map (e.g. *"How do people manage their finances?"* → map the financial management journey) |
| **Target User** | The subject of the human question identifies who the journey should centre on |
| **Steps & Actions** | The runner-up questions surface adjacent behaviours worth including as journey steps |
| **Pain Points** | Clusters from Step 3 highlight the problem areas to probe in the journey |
| **Opportunities** | The gap between the business question and human question reveals where unmet needs likely sit |

> **Suggested User Journey Map scenario** *(generated by DesignSprintAgent from the chosen human question)*:
>
> _(DesignSprintAgent generates a suggested scenario statement here, e.g. "Trace the journey of [target user] as they [action implied by the human question], from [starting trigger] to [end outcome].")_

---

## Notes & Observations

> *(Any tensions surfaced during the session, alternative questions worth revisiting, dissenting views, or follow-up actions the group identified.)*

_(DesignSprintAgent records observations from the chat discussion here)_

---

> **Next Step:** Take the Chosen Human Question and Session Summary into the **User Journey Map** activity.  
> Invoke `@DesignSprintAgent start User Journey Map` to continue Phase 1.
