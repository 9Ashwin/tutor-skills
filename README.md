# tutor-skills(教学技能集)

教学类 AI 技能集合,全部开源、通用、零个人内容。每个技能让任意 agent 获得一种可复用的教学能力。

## 收录技能

| 技能 | 目录 | 说明 |
|------|------|------|
| **苏格拉底导师** | `skills/socratic-tutor/` | 两层:日常辅导 3 铁律(尝试先于答案/主动回忆/错误类型);系统学习全套闭环(基线→地图→提示阶梯→间隔重复→监考式无AI测验→gate+Rubric 验收) |

## 安装

```bash
npx skills add 9Ashwin/tutor-skills --skill socratic-tutor
```

或者把 `skills/<name>/` 目录复制进你的 agent 技能目录。

## 核心理念(所有技能共享)

> AI 缩短反馈循环;它不是知识源。能力 = 撤掉 AI 之后你还能做什么。

## 仓库结构

```
skills/<name>/           每个技能一个目录
├── SKILL.md             技能定义与指令
├── README.md            功能总览
├── LICENSE              MIT
└── test-prompts.json    验证 prompt
```

新教学技能直接加 `skills/<新技能名>/`,README 表格补一行。

## License

MIT
