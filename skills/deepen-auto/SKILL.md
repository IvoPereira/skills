---
name: deepen-auto
description: "Use when the user invokes /deepen-auto or asks to deepen a task and implement it without asking for approval. Same analysis as /deepen (expert practice, raw material, methods, independent validation, Jim Gray review, synthesis), then implements the full plan immediately, verifying as it goes."
argument-hint: "[task to deepen and implement]"
---

# Deepen (auto-approve)

Same method as [/deepen](../deepen/SKILL.md), but the user has approved implementation in advance: invoking this skill is the "yes". Do not ask the closing question.

## Workflow

1. **Assess and rewrite.** Follow "Find the task", "Assess before rewriting" and "Rewrite the prompt" in [../deepen/SKILL.md](../deepen/SKILL.md). Keep it short: the four observations and the rewritten prompt, scaled to the task.
2. **Jim Gray review.** Follow [../deepen/jim-gray.md](../deepen/jim-gray.md), using the local library in `../deepen/jim-gray-library/` first (no re-downloads). Keep it brief when the fit is weak.
3. **Synthesis and plan.** List the implementation plan in order, with where each item lands, as /deepen does. Mark optional items optional.
4. **Implement immediately.** Execute the whole plan without asking. Work in verifiable slices: after each slice run the relevant tests/build and check the result (screenshots for UI) before moving on. Keep the user informed with short progress lines.
5. **Review and report.** Run the project's review gate if it has one (e.g. AGENTS.md second-review), fix confirmed findings, then report what was built, what was verified, and what remains.

## Limits that still apply

Auto-approval covers the listed plan within the user's request and existing permissions. It does not cover:
- destructive or irreversible actions (deleting user data, force-pushes, overwriting files you have not read);
- outward-facing actions (publishing, sending messages, pushing, deploying to shared systems), unless the request names them;
- scope beyond the request. Note extra ideas as optional follow-ups instead of building them.

If the work is too large for one pass, implement in priority order, keep everything working between slices, and state exactly where you stopped.
