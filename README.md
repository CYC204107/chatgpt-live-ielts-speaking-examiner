# ChatGPT Live IELTS Speaking Examiner

一个面向 **ChatGPT 应用、自定义 GPT 和语音模式** 的雅思口语模拟考试项目。

它可以引导考生完成身份确认、Part 1、Part 2、Part 3 和考后评分，并通过随项目提供的题库进行接近真实流程的 IELTS Speaking 模拟练习。

> 本项目现已公开，任何人都可以查看、下载或克隆。它提供的是练习和估分，不代表官方 IELTS 成绩，也不隶属于 IELTS、British Council、IDP 或 Cambridge。

## 主要功能

- 模拟完整的 IELTS Speaking 三部分考试流程
- 考官主动控制考试进度，一次只问一个问题
- 使用自然、专业且中立的考官表达
- Part 2 题卡与对应的 Part 3 题组保持匹配
- 考试过程中不纠错、不教学、不提前评分
- 答非所问时简短拉回，并继续考试流程
- 考试结束后按照四项标准提供估分和改进建议
- 支持 ChatGPT 文字对话与语音模式
- 文本模式下不会编造发音证据

## 在 ChatGPT 应用中使用

本仓库不会通过 GitHub 自动安装到 ChatGPT。请使用 ChatGPT 的“创建 GPT”功能完成配置。

### 1. 下载项目

你可以直接下载 ZIP：

[Download ZIP](https://github.com/CYC204107/chatgpt-live-ielts-speaking-examiner/archive/refs/heads/main.zip)

也可以克隆仓库：

```bash
git clone https://github.com/CYC204107/chatgpt-live-ielts-speaking-examiner.git
```

### 2. 创建自定义 GPT

1. 登录 ChatGPT。
2. 打开“探索 GPT”或“我的 GPT”。
3. 点击“创建”。
4. 进入“配置”页面。
5. 设置名称、头像、描述和对话开场白。

建议名称：

```text
IELTS Speaking Examiner
```

建议对话开场白：

```text
Start a complete IELTS Speaking mock test.
```

### 3. 配置 Instructions

将 `SKILL.md` 中的考试角色、流程和评分规则整理后粘贴到自定义 GPT 的 **Instructions** 栏。Instructions 应要求考官：

- 主动开始并控制考试流程
- 严格按照 Part 1、Part 2、Part 3 的顺序进行
- 一次只问一个问题
- 正式题目只能来自对应题库
- 完整考试结束前不得纠错或评分
- 考试结束后再提供专业估分与建议

### 4. 上传 Knowledge 文件

将以下文件上传到自定义 GPT 的 **Knowledge**：

```text
references/exam-protocol.md
references/question-bank-part-1.md
references/question-bank-part-2.md
references/question-bank-part-3.md
references/scoring-and-feedback.md
```

`agents/openai.yaml` 是可选的项目元数据，配置 ChatGPT 自定义 GPT 时不需要上传。

### 5. 测试与使用

保存 GPT 后，先在预览窗口完成一轮测试。确认身份检查、三个 Part 的过渡、题库调用和考后评分均正常，再正式使用。

如需更接近真实考试，可以在 ChatGPT 应用中打开该 GPT 后使用语音模式作答。

## 评分标准

完整考试结束后，考官会根据以下四项标准给出专业估分：

1. Fluency and Coherence
2. Lexical Resource
3. Grammatical Range and Accuracy
4. Pronunciation

如果只有文字回答，Pronunciation 只能标记为暂定结果，不能作为可靠的正式发音评分。

## 项目结构

```text
chatgpt-live-ielts-speaking-examiner/
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

## 使用建议

- 严格模拟时，不要在考试中途要求范文、翻译或纠错。
- 使用语音模式能够提供更真实的口语考试体验。
- 开始新一轮考试时，可以要求避开近期使用过的话题。
- 正式分享自定义 GPT 前，请先测试题库文件是否能被正确读取。
- 不要在身份检查中提交真实证件号码、住址或其他敏感信息。

## 公开使用与内容说明

本仓库公开提供下载和学习使用。公开访问不代表可以忽略题库、图片、品牌名称或其他第三方内容可能具有的版权和使用限制。请仅在拥有相应权利或获得授权的范围内复制、修改和传播内容。

如果你基于本项目创建公开的自定义 GPT，请遵守 OpenAI 的产品规则、内容政策和分享要求。

---

# English Version

An IELTS Speaking mock-exam project designed for the **ChatGPT app, custom GPTs, and voice mode**.

It guides candidates through the identity check, Part 1, Part 2, Part 3, and a post-test score report while using the included question banks to deliver a realistic IELTS Speaking practice experience.

> This repository is public and may be viewed, downloaded, or cloned by anyone. It is intended for practice and estimated assessment only. It does not provide an official IELTS score and is not affiliated with IELTS, the British Council, IDP, or Cambridge.

## Features

- Simulates the complete three-part IELTS Speaking test
- Proactively manages the test and asks one question at a time
- Uses a natural, professional, and neutral examiner style
- Keeps each Part 2 cue card linked to its matching Part 3 set
- Provides no correction, coaching, or scoring before the test ends
- Redirects clearly irrelevant answers without breaking the test flow
- Provides evidence-based estimated bands and improvement advice
- Supports both text conversations and ChatGPT voice mode
- Never invents pronunciation evidence in text-only sessions

## Use with the ChatGPT App

This GitHub repository does not install itself into ChatGPT. Configure it through ChatGPT's custom GPT builder.

### 1. Download

[Download ZIP](https://github.com/CYC204107/chatgpt-live-ielts-speaking-examiner/archive/refs/heads/main.zip)

Or clone the repository:

```bash
git clone https://github.com/CYC204107/chatgpt-live-ielts-speaking-examiner.git
```

### 2. Create a Custom GPT

1. Sign in to ChatGPT.
2. Open Explore GPTs or My GPTs.
3. Select Create.
4. Open the Configure page.
5. Add a name, icon, description, and conversation starter.

Suggested name:

```text
IELTS Speaking Examiner
```

Suggested conversation starter:

```text
Start a complete IELTS Speaking mock test.
```

### 3. Configure Instructions

Adapt the examiner role, test procedure, and scoring rules from `SKILL.md` and place them in the custom GPT **Instructions** field. The instructions should require the examiner to:

- Start and manage the test proactively
- Follow Part 1, Part 2, and Part 3 in order
- Ask one question at a time
- Use formal questions only from the corresponding banks
- Give no correction or score before the full test ends
- Provide professional assessment and advice after the formal ending

### 4. Upload Knowledge

Upload these files to the custom GPT **Knowledge** section:

```text
references/exam-protocol.md
references/question-bank-part-1.md
references/question-bank-part-2.md
references/question-bank-part-3.md
references/scoring-and-feedback.md
```

`agents/openai.yaml` contains optional project metadata and is not required when configuring a custom GPT.

### 5. Test and Use

Save the GPT and complete a preview test. Confirm that the identity check, transitions, question-bank selection, and final assessment work correctly before regular use.

For a more realistic speaking experience, open the custom GPT in the ChatGPT app and answer through voice mode.

## Assessment Criteria

After the complete test, the examiner provides estimated results for:

1. Fluency and Coherence
2. Lexical Resource
3. Grammatical Range and Accuracy
4. Pronunciation

In text-only sessions, Pronunciation must remain provisional and should not be presented as a reliable official-style pronunciation score.

## Repository Structure

```text
chatgpt-live-ielts-speaking-examiner/
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

## Recommendations

- During a strict mock test, do not request model answers, translation, or correction before the test ends.
- Voice mode provides a more realistic speaking-test experience.
- When starting another test, ask the examiner to avoid recently used topics.
- Test Knowledge retrieval before sharing the custom GPT publicly.
- Never submit real identity-document numbers, addresses, or other sensitive information during the simulated identity check.

## Public Use and Content Notice

This repository is publicly available for download and study. Public availability does not override copyright or usage restrictions that may apply to question-bank materials, images, trademarks, or other third-party content. Copy, modify, and redistribute material only when you have the necessary rights or permission.

If you publish a custom GPT based on this project, follow OpenAI's applicable product rules, content policies, and sharing requirements.
