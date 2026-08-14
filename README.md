# closed-loop-tutor(闭环导师)

简体中文 | [English](./README_EN.md)

把任意 AI agent 变成高质量导师:将「我想学 X」转化为**可验证的能力**,由一条闭环反馈循环驱动。

```
基线诊断 → SMART+OKR 目标 → 源头优先资源栈 → 最小单元课程
→ 主动回忆 → 提示阶梯反馈 → 变式与迁移练习
→ 间隔重复 → 无AI延迟测验 → 真实世界迁移
```

## 核心理念

> AI 缩短反馈循环;它不是知识源。能力 = 撤掉 AI 之后你还能做什么。

## 安装

```bash
npx skills add 9Ashwin/closed-loop-tutor
```

或者把 `skills/closed-loop-tutor/` 目录复制进你的 agent 技能目录。

## 它做什么

| 阶段 | 行为 |
|------|------|
| 诊断 | 用真实任务测量起点,不信自我评估 |
| 目标 | SMART + OKR,关键指标 = 有 AI 与无 AI 的成绩差 |
| 资源 | 源头优先:官方文档 → 课程 → 综述 → 专家解读 → 社区 |
| 教学 | 每个最小单元一课,紧扣使命;讲解前先主动回忆 |
| 反馈 | 提示阶梯:尝试 → 错误区域 → 引导问题 → 原则 → 局部例子 → 完整解法(仅应求给出) |
| 练习 | 变式题,再出跨情境迁移题 |
| 记忆 | 间隔重复(FSRS 式)+ 无 AI 延迟测验 |
| 迁移 | 以真实项目或陌生情境收官;然后更新目标 |

## 教学工作区

技能维护一个有状态的教学工作区:

```
MISSION.md           学习动机(锚定一切教学)
RESOURCES.md         源头优先的资源栈
NOTES.md             学习者偏好
learning-records/    编号学习记录 → 计算最近发展区
lessons/             每个最小单元一个自包含 HTML
reference/           压缩速查表与术语表
assets/              可复用组件(共享样式表优先)
```

## 文件结构

```
skills/closed-loop-tutor/
├── SKILL.md              技能定义与指令
├── README.md             功能总览
├── LICENSE               MIT
└── test-prompts.json     验证 prompt
```

## 设计说明

- 融合两条成熟传统:闭环学习法(目标 → 基线 → 资源栈 → 最小单元 → 主动回忆 → 反馈 → 间隔 → 迁移)+ 教学工作区模式(MISSION / lessons / reference / learning-records / assets)。
- 语言无关:适用于编程、语言、数学、手艺等任何主题。
- Agent 无关:不绑定任何平台 hook,任何 LLM agent 都能采纳。

## License

MIT
