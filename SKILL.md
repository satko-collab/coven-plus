---
name: coven-plus
description: Orchestrate a disciplined panel of distinct expert voices that independently assess a consequential problem, cross-examine one another, revise their positions, and produce a narrator synthesis benchmarked against a simple direct answer. Use whenever the user invokes COVEN+, asks for an expert panel, coordinated or orchestrated voices, multi-perspective deliberation, structured cross-examination, devil’s-advocate testing, or a p/a quality audit. Also use for contested, expensive, high-stakes, or hard-to-reverse decisions where several kinds of expertise or values materially interact. Use LIGHT mode or a direct answer for routine, reversible, easily checked tasks. Do not treat simulated voices as independent evidence or manufacture disagreement.
---

# COVEN+

*Coordinated & Orchestrated Voices for Expert Navigation + Meta-Interpretive Reasoning Layer*

## Core contract

Transform the user’s request into a compact structured brief, then execute it. Use the language of the task. Help the user think rather than replace their judgment.

Distinguish throughout:

- facts;
- assumptions;
- values;
- preferences;
- unknowns.

Never invent a citation, stakeholder, consensus, or numerical weighting.

## Select the effort level

Use **FULL mode** when the decision is consequential, contested, expensive, high-stakes, or difficult to reverse.

Use **LIGHT mode** when the task is moderately consequential but benefits from contrasting perspectives. Use a direct answer when the task is routine, reversible, or easily checked.

If the user explicitly requests FULL or LIGHT mode, follow that request unless safety or feasibility requires otherwise. Do not use panel complexity merely because the topic sounds intellectual.

## Build the task brief

State or infer:

- **Task:** what must be answered or produced;
- **Purpose or decision:** what the result will be used for;
- **Audience:** who must understand or act on it;
- **Constraints:** time, policy, resources, jurisdiction, tools, or model limitations;
- **Useful output:** the form that can be acted on.

Ask a clarifying question only when the answer would materially change the panel composition, decision criterion, or safe course of action. Otherwise state reasonable assumptions and proceed.

## Start with Meta-Reading

Open with a section titled **Meta-Reading** in three to five concise lines. State:

1. what output would actually help;
2. what expertise is most relevant;
3. what format is most useful;
4. what level of detail is sufficient.

Show only a concise task interpretation, never private chain-of-thought. Do not repeat this section later.

## Design the panel

### FULL mode

Create exactly four distinct voices unless the user explicitly requests a different number. Use roles supplied by the user. If none are supplied, use:

1. domain generalist;
2. methodologist;
3. risk analyst;
4. exactly one devil’s advocate.

### LIGHT mode

Create exactly three voices, including one voice responsible for material challenge. Use one challenge round and a short synthesis.

For each voice specify:

- a memorable name or role;
- what it protects;
- what evidence it trusts;
- its likely blind spot;
- one question, observation, or falsifier that could change its mind.

Make the voices structurally different. Do not create four paraphrases of the same expert. The devil’s advocate must challenge claims rather than people and must not manufacture opposition.

## Run independent first passes

Before cross-examination, make each voice produce an independent first pass using only the task brief and its own role specification. Include:

- recommendation;
- assumptions;
- reasons and available evidence;
- main uncertainty;
- provisional **p** and **a** marks, each with a one-line reason.

Treat this independence as a reasoning simulation, not as independent testimony or evidence. Never increase confidence merely because several voices produced by the same model agree.

## Cross-examine

In FULL mode, require each voice to:

1. name the strongest claim made by another voice;
2. challenge one material claim with a counterexample, missing stakeholder, competing mechanism, or verification request;
3. state what evidence would change its mind.

In LIGHT mode, run one compact challenge round covering the most consequential disagreement or untested assumption.

Do not reward performative conflict. Spend challenge effort where an error would change the decision.

## Revise

After cross-examination, require each voice to state what it:

- kept;
- changed;
- rejected.

Do not force consensus. Preserve material disagreement, minority insights, and incompatible value choices.

## Synthesize as Narrator

Produce:

1. agreements;
2. material conflicts;
3. resolved points and unresolved choices;
4. unique or minority insights;
5. a verification checklist;
6. one recommendation plus meaningful alternatives.

Separate facts, assumptions, values, preferences, and unknowns. Identify the decision owner when relevant; the panel advises but does not appropriate the user’s judgment.

## Benchmark the added complexity

State the simplest credible direct-answer baseline. Compare the panel’s recommendation with:

- that baseline;
- the user’s stated criteria;
- the strongest minority position.

Then answer explicitly:

> Did the added complexity change the answer, make a material claim more checkable, reveal a neglected stakeholder or trade-off, or merely produce more text?

If the panel adds no material value, say so and recommend the direct answer.

Do not claim undefined weights, invisible scoring, independent-agent evidence, or hidden budgeting calculations.

## Finish with the p/a audit

Give two public working marks in **[0,1]**:

- **p — epistemic confidence:** support from evidence, sources, logic, and current knowledge;
- **a — adequacy:** fit to the purpose, audience, format, language, constraints, and required depth.

For each mark provide:

- one reason;
- the largest uncertainty or mismatch;
- the next verification step or correction.

When **p < 0.70**, name the uncertainty and verification route. When **a < 0.70**, name the mismatch and correction. When the marks diverge, explain why.

Treat these marks as working judgments, not calibrated probabilities or measurements.

## Default output order

Use:

**Meta-Reading → panel design → independent voices → cross-examination → revisions → Narrator synthesis → recommendation and alternatives → direct-answer benchmark → p/a audit**

Compress sections in LIGHT mode. Prefer a usable result over ritual completeness.

## Methodological safeguards

- Do not treat several voices from one model as independent evidence.
- Do not cite agreement as proof; agreement may reflect shared training data or shared blind spots.
- Do not let the devil’s advocate create a false balance against well-supported evidence.
- Do not replace source verification with panel deliberation.
- For medical, legal, financial, safety-critical, or other high-stakes matters, verify current authoritative sources and preserve the boundary between deliberation and professional judgment.
- Do not expose private chain-of-thought. Give conclusions, concise reasons, assumptions, evidence, and uncertainty.
- Stop escalating complexity when the direct baseline already meets the user’s criteria and the panel produces no decision-relevant difference.

## Authorship and provenance

**Creator:** Dr Piotr Kowzan, University of Gdańsk  
**Contact:** piotr.kowzan@ug.edu.pl  
**License:** Creative Commons Attribution 4.0 International (CC BY 4.0)

The decision architecture is inspired by multi-expert prompting. The Meta-Reading layer is adapted from a meta-prompt presented by Nate B. Jones. Read [references/provenance.md](references/provenance.md) when citing, auditing, or modifying the method.

When updating this skill, consult the preserved [original prompt](references/original-prompt.md) and run the [evaluation cases](references/evaluation-cases.md). During ordinary use, load those files only when provenance, maintenance, or boundary testing is relevant.
