# Closed-Loop Tutor Skill

Turn any AI agent into a high-quality tutor that converts "I want to learn X" into verifiable ability, driven by a closed feedback loop.

## The Core Belief

> AI shortens the feedback loop; it is not the knowledge source. Ability = what you can still do after removing the AI.

## Features

- **Baseline diagnosis first** — measures the real starting point with a task, not self-report
- **Dual-layer goals** — SMART (specific/measurable/achievable/relevant/time-bound) + OKR (outcomes not activities), with the critical with-AI vs without-AI gap metric
- **Source-first resource stack** — official docs → authoritative courses → quality surveys → expert explanations → community; primary sources kept in original language
- **Minimal unit lessons** — one tightly-scoped, mission-tied lesson per unit, one tangible win each
- **Active recall before explanation** — the learner recalls before being taught
- **Hint ladder feedback** — attempts → error region → guiding question → principle → local example → full solution (only on request)
- **Error taxonomy** — concept gap / missing condition / false analogy / computational / strategy / carelessness
- **Variant + transfer exercises** — same concept rephrased, then cross-context
- **Spaced repetition + no-AI delayed tests** — FSRS-style intervals; mastery = what survives without AI
- **Real-world transfer as the finish line** — apply to a real project or novel context
- **Stateful teaching workspace** — MISSION / RESOURCES / NOTES / learning-records / lessons / reference / assets

## Usage

Trigger with prompts like:

- "Teach me X" / "教我 X"
- "How do I learn Y?" / "怎么学 Y"
- "Make me a study plan for Z" / "学习计划"
- "Tutor me on ..." / "辅导我 ..."
- "I want to learn X" / "我想学 X"

The skill is self-contained: it creates and maintains the teaching workspace, runs the closed loop, and grades with rubrics.

## Files

- `SKILL.md` — Skill definition and instructions
- `test-prompts.json` — Test prompts for validation

## Design Notes

- Combines two established traditions: the closed-loop learning method (goal → baseline → resource stack → minimal units → active recall → feedback → spacing → transfer) and the teach workspace pattern (MISSION / lessons / reference / learning-records / assets).
- Language-agnostic: works for programming, languages, math, crafts, anything.
- Agent-agnostic: no platform-specific hooks; any LLM agent can adopt it.

## License

MIT
