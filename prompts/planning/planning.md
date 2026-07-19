# Planning Prompts

Use these prompts to help an AI agent assist with breaking down tasks, creating plans, and structuring work.

---

## Break Down a Large Task

```
I need to accomplish the following goal:

**Goal:** [DESCRIBE THE GOAL]
**Context:** [RELEVANT BACKGROUND — tech stack, constraints, team size, deadline, etc.]

Please break this down into concrete, actionable sub-tasks. For each sub-task:
- State what needs to be done
- Estimate the relative effort (small / medium / large)
- Note any dependencies on other sub-tasks
- Flag any risks or unknowns

Present the result as an ordered list or a dependency graph if appropriate.
```

---

## Create a Project Plan

```
Help me create a project plan for the following:

**Project:** [PROJECT NAME / DESCRIPTION]
**Goal / success criteria:** [WHAT DOES DONE LOOK LIKE?]
**Timeline:** [AVAILABLE TIME OR DEADLINE]
**Resources:** [TEAM SIZE, KEY SKILLS AVAILABLE]
**Known constraints:** [BUDGET, TECHNICAL LIMITATIONS, ETC.]

Provide:
1. A list of milestones with approximate dates
2. Key deliverables for each milestone
3. Identified risks and mitigation strategies
4. Open questions that need answers before work can begin
```

---

## Prioritize a Backlog

```
I have the following list of tasks / features and need help deciding what to work on first.

**Context / goal:** [WHAT ARE YOU OPTIMIZING FOR — e.g. user impact, risk reduction, revenue]

<backlog>
[LIST YOUR TASKS / STORIES HERE]
</backlog>

Please prioritize them using [FRAMEWORK, e.g. "MoSCoW — four levels: Must have, Should have, Could have, Won't have this time", "RICE scoring (Reach, Impact, Confidence, Effort)", or "your own judgment"] and explain the reasoning behind the top 3–5 items.
```

---

## Define Acceptance Criteria

```
Please write clear acceptance criteria for the following feature or user story:

**Feature:** [DESCRIBE THE FEATURE]
**User role:** [WHO IS USING THIS?]
**Goal:** [WHAT DO THEY WANT TO ACHIEVE?]

Use the "Given / When / Then" format for each criterion. Cover the happy path, edge cases, and error states.
```

---

## Retrospective Facilitation

```
Help me run a retrospective for [PROJECT / SPRINT / PERIOD].

**What happened:** [BRIEF SUMMARY OF THE WORK]
**Team size:** [NUMBER OF PEOPLE]
**Format:** [e.g. Start / Stop / Continue — or leave blank for a suggestion]

Please:
1. Suggest a set of retrospective questions to ask the team
2. Provide a structure for the session (timing, activities)
3. Give tips for facilitating productive discussion and actionable outcomes
```

---

## Risk Assessment

```
I'm planning to [DESCRIBE WHAT YOU PLAN TO DO]. Help me identify and assess the risks.

For each risk, provide:
- A description of the risk
- Likelihood (low / medium / high)
- Impact if it occurs (low / medium / high)
- A risk score (rate likelihood and impact as 1 = low, 2 = medium, 3 = high; risk score = likelihood * impact, max 9)
- Recommended mitigation or contingency plan

Sort the risks from highest to lowest risk score.
```
