# IELTS Speaking Examiner

一个用于 Codex 的 IELTS Speaking 模拟考试 Skill。它按照完整的口语考试流程组织身份确认、Part 1、Part 2、Part 3 以及考后评分，并优先使用随 Skill 提供的题库。

> 本项目提供的是练习与能力评估，不代表官方 IELTS 成绩，也不隶属于 IELTS、British Council、IDP 或 Cambridge。

## 主要功能

- 模拟完整的 IELTS Speaking 三部分考试流程
- 考试过程中一次只问一个问题
- 使用自然、专业且中立的考官表达
- Part 2 题卡与对应的 Part 3 题组保持匹配
- 考试结束前不纠错、不教学、不提前评分
- 按四项口语评分标准提供专业估分和改进建议
- 文本模式下不会编造发音证据

## 目录结构

```text
ielts-speaking-examiner/
├─ SKILL.md
├─ agents/
│  └─ openai.yaml
└─ references/
   ├─ exam-protocol.md
   ├─ question-bank-part-1.md
   ├─ question-bank-part-2.md
   ├─ question-bank-part-3.md
   └─ scoring-and-feedback.md
```

## 安装

该仓库是私有仓库，因此只有仓库所有者或获得授权的协作者可以克隆。

在已经登录 GitHub CLI 的 Windows PowerShell 中运行：

```powershell
git clone https://github.com/CYC204107/ielts-speaking-examiner.git "$HOME\.codex\skills\ielts-speaking-examiner"
```

如果你的 Codex 使用其他个人 Skill 目录，请将整个仓库复制到对应目录，并重新启动 Codex 或开始一个新任务。

## 使用方法

在 Codex 中可以直接提出类似请求：

```text
请使用 IELTS Speaking Examiner 为我进行一次完整的雅思口语模拟考试。
```

也可以明确调用：

```text
$ielts-speaking-examiner 开始一场完整的雅思口语模拟考试。
```

考试开始后，按照考官的问题逐题作答。完整考试结束后，Skill 会根据以下四项标准给出估分：

1. Fluency and Coherence
2. Lexical Resource
3. Grammatical Range and Accuracy
4. Pronunciation

## 使用建议

- 使用语音输入能提供更接近真实口语考试的体验。
- 如果只有文字回答，发音评分只能作为暂定结果。
- 严格模拟时不要在考试中途要求范文或纠错。
- 在同一任务中重新考试时，可以要求避开之前使用过的话题。

## 内容说明

题库及参考资料仅用于个人学习和模拟练习。请勿在没有相应权利或授权的情况下公开传播受版权保护的内容。建议继续保持该仓库为私有状态。

## License

No license is currently granted for redistribution. All rights are reserved unless explicitly stated otherwise.
