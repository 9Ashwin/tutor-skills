# closed-loop-tutor

简体中文 | English

Turn any AI agent into a high-quality tutor that converts "I want to learn X" into verifiable ability, driven by a closed feedback loop.

```
Baseline diagnosis → SMART+OKR goals → Source-first resource stack → Minimal unit lessons
→ Active recall → Hint-ladder feedback → Variant & transfer exercises
→ Spaced repetition → No-AI delayed tests → Real-world transfer
```

## The Core Belief

> AI shortens the feedback loop; it is not the knowledge source. Ability = what you can still do after removing the AI.

## Installation

```bash
npx skills add 9Ashwin/closed-loop-tutor
```

Or copy `skills/closed-loop-tutor/` into your agent's skills directory.

## What it does

| Phase | Behavior |
|-------|----------|
| Diagnose | Measures the real starting point with a task, not self-report |
| Goal | SMART + OKR with the with-AI vs without-AI gap as the critical metric |
| Resources | Source-first stack: official docs → courses → surveys → experts → community |
| Teach | One minimal, mission-tied lesson per unit; active recall before explanation |
| Feedback | Hint ladder: attempt → error region → guiding question → principle → example → solution (only on request) |
| Practice | Variant problems, then cross-context transfer problems |
| Retain | Spaced repetition (FSRS-style) + no-AI delayed tests |
| Transfer | Real project or novel context as the finish line; then update the goal |

## Workspace

The skill maintains a stateful teaching workspace:

```
MISSION.md           why they are learning (grounds everything)
RESOURCES.md         source-first resource stack
NOTES.md             learner preferences
learning-records/    numbered records → zone of proximal development
lessons/             one self-contained HTML per minimal unit
reference/           compressed cheat sheets & glossaries
assets/              reusable components (shared stylesheet first)
```

## Files

```
skills/closed-loop-tutor/
├── SKILL.md              skill definition & instructions
├── README.md             feature overview
├── LICENSE               MIT
└── test-prompts.json     validation prompts
```

## License

MIT
