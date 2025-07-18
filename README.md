# LLM-Chinese-Semantic-Comprehension

本项目旨在比较不同中文大语言模型（LLMs）在处理语义理解类问题时的表现差异。通过设计包含语言歧义、双关语、绕口令、多义词等特征的问题，分析模型对中文语义细节的把握能力，展示其语言推理与表达逻辑的优劣。

---

## 🧪 项目背景

中文语义理解是语言模型能力评估中的重要组成部分，尤其是在应对模糊、含混、讽刺、多层指代等语言现象时。为了评估当前主流中文大模型在这些方面的能力，我们选取了以下两个模型进行对比：

- 智谱 **ChatGLM3-6B**
- 通义 **千问 Qwen-7B-Chat**

---

## 📁 项目结构

    LLM-Chinese-Semantic-Comprehension
    │ .gitignore # Git 忽略规则
    │ LLM部署报告.docx # 文档与详细分析说明
    │ README.md # 项目说明文件
    │
    ├── 智谱ChatGLM3-6B
    │   ├── git截图.png # 模型部署截图
    │   └── 测试结果截图.png # 对话结果截图
    │
    └── 通义千问Qwen-7B-Chat
        ├── git截图.png # 模型部署截图
        └── 测试结果截图.png # 对话结果截图

---

## 🧠 模型介绍

### 🟩 ChatGLM3-6B
- 开发者：智谱 AI
- 模型语言：中文优化，支持多轮对话
- 优势：结构清晰，表达直接
- 局限：推理链条短，语言处理偏句法层面

### 🟦 Qwen-7B-Chat
- 开发者：阿里达摩院
- 模型语言：中文优先，含语言理解强化训练
- 优势：语境感强，表达深入，解释倾向全面
- 局限：回答略显啰嗦，结构偶有跳跃

---

## 📝 测试样例及分析

测试问题涵盖：
- 多义表达（如“谁都看不上”）
- 语义重复（如“能穿多少穿多少”）
- 指代链追踪（如“他知道我知道你知道他不知道吗？”）
- 情感判断与语境缺省（如“明明明明明白白白喜欢他”）
- 多义词使用（如“意思”的多种语境）

详细分析可见文档：
- `LLM部署报告.docx`

模型具体输出结果截图位于对应模型文件夹下的：
- `git截图.png`
- `测试结果截图.png`

---

## 📊 总结与对比

| 维度             | ChatGLM3-6B             | Qwen-7B-Chat               |
|------------------|--------------------------|----------------------------|
| 表达简洁性       | ✅ 强                     | ⚠️ 略显啰嗦                 |
| 语义理解深度     | ⚠️ 中等偏浅               | ✅ 深入                     |
| 语言组织逻辑     | ⚠️ 易混乱                 | ✅ 结构清晰                 |
| 适合使用场景     | 快速问答、句法分析       | 教学演示、语用推理         |

---

## 📌 使用建议

- 需要快速、直接回答的使用者可优先考虑 ChatGLM3-6B。
- 对语言细节理解与扩展要求更高的场景可选择 Qwen-7B-Chat。
