# tutor-skills · Socratic Tutor

Turn any AI agent into a tutor that actually teaches: converting "I want to learn X" into verifiable ability, not "sounds like I understood it".

```
Attempt before answer → Active recall → Hint-ladder feedback → Error taxonomy → Variant & transfer exercises
→ Spaced repetition queue → Proctored no-AI tests → Gate checkpoint → Real-world transfer
```

## Core Belief

> AI shortens the feedback loop; it is not the knowledge source. Ability = what you can still do after removing the AI.

The biggest failure of AI tutoring is **fluency illusion** — with AI present, everything works; without AI, nothing works. Every mechanism in this skill fights that: baseline diagnosis measures the real starting point, proctored tests measure real retention, and the gate checkpoint gates progress — even in efficiency mode.

## Two Tiers

**Daily tutoring (default, lightweight)**: three iron rules, no files created — ① attempt before answer ② at least one active-recall check per session ③ one error taxonomy record per mistake. Light enough to actually use.

**Systematic learning (triggered by "systematically learn X" / "make me a course")**: the full closed loop:
- Knowledge map (map.md) → spaced repetition queue (review-queue.md, 3-7-14 days) → proctored no-AI tests (questions/answers separated, one question at a time, graded on the spot) → gate checkpoint (mandatory in all modes) → real-world transfer
- Clear trigger boundaries: "系统学 X / 做套课程 / 学习计划" → systematic; "这是什么 / 帮我看看 / 为什么报错" → daily

## Install

```bash
npx skills add 9Ashwin/tutor-skills --skill socratic-tutor
```

Or copy `skills/socratic-tutor/` into your agent's skills directory.

## Core Mechanisms

| Mechanism | Problem it solves | How it lands |
|-----------|-------------------|--------------|
| Hint ladder | Giving answers = learner stops thinking | Five rungs: attempt → error region → guiding question → principle → partial example → (only on request) full solution |
| Active recall | Fluency illusion | Learner recalls/writes from memory before explanation |
| Error taxonomy map | Vague "you're wrong" gives no guidance | Concept gap→reteach, missing condition→boundary variants, false analogy→counterexamples, computation→drill, strategy→expert thinking, careless→checklist |
| Proctored no-AI tests | Open-book self-test ≠ real retention | questions.md separated from answers, one question at a time graded on the spot, with-AI round uses different same-difficulty questions |
| Gate checkpoint | Progress bypassed by efficiency mode | No-AI ≥90% + transfer exercise done independently + explanation graded A,B ≥3 on Rubric; no mode exempt |
| Spaced repetition queue | Storage strength (long-term retention) | review-queue.md tracks 3-7-14 days, due items cleared at session start |
| Rubric grading | Open answers graded by feel | A concept correctness / B reasoning chain / C evidence quality / D unsupported assumptions, 0-4 |

## Structure

```
skills/socratic-tutor/
├── SKILL.md              two-tier design + full closed loop
├── README.md             feature overview
├── LICENSE               MIT
├── test-prompts.json     validation prompts
└── assets/
    └── prompt-ladder.html   hint-ladder component (anchored in lesson footers)
```

## License

MIT
