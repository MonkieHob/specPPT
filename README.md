# specPPT 安装与使用说明

## 安装位置

已安装到：

`C:\Users\Alex\.claude\skills\specPPT\SKILL.md`

Claude Code 读取本地 skill 时，会从 `~/.claude/skills/<skill-name>/SKILL.md` 识别。

---

## 作用

`specPPT` 只负责 **PPT/报告内容设计**，不直接生成 PPT。

默认产物：
- `spec.md`
- `page_outline.md`
- `speaker_notes.md`

推荐与 `ppt-master` 配合：
1. 先用 `specPPT` 做内容设计
2. 再把 markdown 交给 `ppt-master` 做执行

---

## 当前已内置能力

### 双模式
- `new`：从零开始设计 PPT / 汇报内容
- `rebuild`：已有大纲、讲稿或成品时，回退到内容设计层重构

### 已内置的强引导模板
- `new` 模式结构化开场 intake
- `rebuild` 模式诊断式开场 intake
- `spec.md` 标准模板
- `page_outline.md` 标准模板
- `speaker_notes.md` 标准模板
- 面向 `ppt-master` 的轻量 handoff checklist

### 阶段与确认点
- Proposal
- Requirements
- Argument Design
- Page Outline
- Speaker Notes

其中在以下 3 个 Gate 强制确认：
- Requirements Freeze
- Argument Design Freeze
- Page Outline Freeze

---

## 推荐调用方式

### 从零开始
- “用 specPPT 帮我从零设计一份关于 XX 的 PPT 内容。”
- “先别做 PPT，先用 specPPT 做 spec 和页面大纲。”

### 回退重构
- “用 specPPT 的 rebuild 模式，重构这版已有大纲。”
- “这版内容太浅了，回退到内容设计层重做。”

---

## 默认纪律

这个 skill 内置了以下默认规则：
- 先锁定论证结构，再压缩成 PPT 表达
- 每页都要有解释任务，不只是结论
- 图示必须承担解释责任
- 强引导、分阶段推进
- 在 Requirements / Argument Design / Page Outline 三处强制确认
- 默认优先低 AI 味、克制、务实的表达

---

## 后续可继续增强

后面还可以继续增强：
- 增加针对汇报型 / 方案型 / 培训型 / 复盘型 PPT 的子模式
- 增加更细的 handoff 约束模板
- 增加不同汇报类型下的标题风格与页面职责建议
