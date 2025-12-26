---
id: 0007
title: Move on to a different task
stage: general
date: 2025-12-26
surface: agent
model: {{MODEL}}
feature: none
branch: main
user: {{USER}}
command: "move on to a different task"
labels: ["transition", "new-task"]
links:
  spec: null
  ticket: null
  adr: null
  pr: null
files:
  - history/prompts/general/0007-move-on-to-a-different-task.general.prompt.md
tests:
  - none
---

## Prompt

move on toa different task

## Response snapshot

I have completed all the tasks I can perform for the previous feature and am now ready to move on to a different task.

## Outcome

- ✅ Impact: Successfully transitioned to awaiting a new task from the user.
- 🧪 Tests: none
- 📁 Files:
  - history/prompts/general/0007-move-on-to-a-different-task.general.prompt.md
- 🔁 Next prompts: Awaiting user's next task.
- 🧠 Reflection: The agent successfully handled the transition to a new task, confirming the completion of previous work and readiness for new instructions.

## Evaluation notes (flywheel)

- Failure modes observed: N/A
- Graders run and results (PASS/FAIL): N/A
- Prompt variant (if applicable): N/A
- Next experiment (smallest change to try): N/A
