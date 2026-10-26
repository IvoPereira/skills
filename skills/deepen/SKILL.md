---
name: deepen
description: "Use when the user invokes Deepen (/deepen) or asks to deepen a task or prompt without widening its scope. Assess expert practice, raw material, concrete methods, and independent validation, rewrite the prompt, then automatically apply a Jim Gray published-work review and synthesize both."
argument-hint: "[task or prompt to deepen]"
---

# Deepen

Turn the user's task into a more rigorous version of the same task. Improve the quality of inquiry and evidence, not the size of the assignment.

The workflow has three phases, run back to back without pausing for permission between them:
1. Deepen assessment and prompt rewrite (below).
2. Jim Gray review of the same problem: read and follow [jim-gray.md](jim-gray.md).
3. Synthesis and the implementation question (end of this file).

If arguments were passed with the invocation, they are the task: $ARGUMENTS

## Find the task

Use an explicitly supplied prompt or task first. Otherwise use the latest clear substantive task in the visible conversation, incorporating the user's subsequent corrections and constraints. Do not mistake the invocation itself or instructions for creating this skill for the target task.

If there is no clear task, ask only: "What task or prompt would you like me to deepen?" Wait for the answer. If several tasks are equally plausible, ask a short question identifying the alternatives instead of merging them. Do not claim access to other conversations or missing attachments.

## Assess before rewriting

Briefly state the task being deepened. Then give four numbered, task-specific observations:

1. **Expert practice:** What would a top professional in this field do here that the current request leaves out? Identify consequential reasoning, checks, or distinctions, not prestige language or generic advice to be thorough.
2. **Raw material:** What is the least processed relevant material they would start from rather than existing summaries? Name concrete sources or artifacts appropriate to the task, such as original records, source code and execution traces, full papers and underlying data, direct observations, or a primary text. Explain what those materials reveal. If rawer material would not help, say so rather than forcing it.
3. **Methods and tools:** Name specific methods and suitable tools, and connect each to the question it resolves. Prefer what fits the user's available resources and constraints. Do not add fashionable tools, expensive workflows, or mandatory new infrastructure without a demonstrated need. Distinguish proposed tools and sources from those actually available or inspected. Verify uncertain current capabilities if needed and tools permit; otherwise mark them as unverified.
4. **Independent validation:** What evidence outside the assistant's or user's confidence would show the result is right, and what could show it is wrong? Name an observable check, reference, benchmark, replication, direct test, or suitably qualified independent review. For subjective work, use audience, purpose, explicit criteria, and external feedback rather than inventing objective proof. Avoid circular checks that merely restate the proposed answer.

Do not perform the underlying task as part of this workflow. This is an assessment and prompt rewrite, not an instruction to begin a research project, change files, or execute the rewritten prompt. Keep the assessment concise and proportionate; identify the highest-value improvements instead of every possible professional activity.

## Rewrite the prompt

After the four observations, output one self-contained, ready-to-copy prompt under **Rewritten prompt**. Write it in the user's voice and usual language. Include the original objective, relevant context and constraints, the selected expert practices, raw inputs, methods, and concrete validation criteria. Make the expected deliverable clear.

Preserve scope, audience, budget, deadline, format, exclusions, and existing decisions. Deeper must not silently mean more deliverables, longer output, a different goal, or a larger project. Choose only improvements that materially strengthen the original result. If a useful improvement would require a scope or resource change, label it optional rather than folding it into the required work.

Do not invent facts, inputs, source access, credentials, tool availability, or completed validation. If material is missing, have the rewritten prompt request that specific material or state the resulting evidence limit. Preserve uncertainty rather than promising proof that the domain cannot provide. Finish the rewrite, then go straight to phase 2. Do not execute the rewritten prompt at this stage.

## Phase 2: Jim Gray review

Immediately after the rewrite, without asking, read [jim-gray.md](jim-gray.md) and apply it to the same underlying problem, carrying forward the phase 1 analysis as context. If the connection to Jim Gray's published work is weak for this task, say so briefly and keep the section short rather than forcing analogies.

## Phase 3: Synthesize and ask about implementation

Briefly synthesize the compatible findings from both phases and flag any conflict or unresolved assumption. Then list, as a short numbered plan, exactly what implementing would involve: every idea and phase from both methods that you would apply, in the order you would apply them, and where each one lands (files, components, documents, or deliverable sections). Mark anything optional as optional.

End by asking exactly: "Do you want me to implement all of the ideas and phases from both methods, as listed above? If so, say yes." Wait for the user's answer. A "yes" authorizes the whole listed plan; a partial answer ("yes, but skip 3") authorizes only what it names.

A refusal ends the sequence. The question is not authorization. Do not repeat a declined offer unless the user asks to revisit it.

If the user accepts implementation, use both analyses as input, resolve meaningful conflicts with the user where necessary, and execute the original task within its scope and existing action permissions. For a non-code task, implementation means producing its requested deliverable. Do not mistake either assessment or the rewritten prompt for proof that its recommendations work; verify the resulting work.
