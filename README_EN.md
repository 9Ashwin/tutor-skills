# tutor-skills

A collection of open-source teaching skills for AI agents — generic, reusable, no personal content.

## Skills

| Skill | Directory | Description |
|-------|-----------|-------------|
| **Socratic Tutor** | `skills/socratic-tutor/` | Two tiers: daily tutoring = 3 iron rules (attempt before answer / active recall / error taxonomy); systematic learning = full closed loop (baseline → map → hint ladder → spaced repetition → proctored no-AI tests → gate with Rubric grading) |

## Install

```bash
npx skills add 9Ashwin/tutor-skills --skill socratic-tutor
```

Or copy the `skills/<name>/` directory into your agent's skills directory.

## Core Belief

> AI shortens the feedback loop; it is not the knowledge source. Ability = what you can still do after removing the AI.

## Structure

```
skills/<name>/           one directory per skill
├── SKILL.md             skill definition & instructions
├── README.md            feature overview
├── LICENSE              MIT
└── test-prompts.json    validation prompts
```

Add a new teaching skill by dropping a directory under `skills/` and adding one row to the README table.

## License

MIT
