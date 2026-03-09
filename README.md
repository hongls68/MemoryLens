# 🕶️ MemoryLens - 记忆透镜

> 独居老人的“第二大脑”：跌倒秒级报警，遗忘瞬间回溯。

---

## 🎯 项目简介

**MemoryLens** 是一款专为独居老人设计的 AI 驱动智能穿戴辅助系统。它不仅仅是一个监控设备，更是老人的“视觉外脑”，旨在通过多模态大模型解决**安全监测**、**记忆辅助**及**情感陪伴**三大核心痛点，让子女安心，让老人舒心。

### ✨ 核心功能
- 🚨 **第一视角危险预警** - 佩戴式摄像头实时监测跌倒/火灾/异常静止，**5秒内**推送视频警报给子女。
- 🔍 **视觉记忆回溯** - 支持自然语言问答（如：“我眼镜放哪了？”），AI 自动检索过去1小时视频流并定位物体。
- 💬 **场景化主动交互** - 识别老人行为意图（如对着药瓶发呆），主动语音提醒服药步骤，提供有温度的陪伴。

### 🧠 AI 技术栈
- **多模态大模型 (MLLM)**: 基于 Qwen-VL-2026，深度理解视频场景与物体关系。
- **端侧小模型 (SLM)**: 低功耗芯片本地运行跌倒检测，保障隐私与低延迟。
- **RAG (检索增强生成)**: 构建个人短期记忆库，实现精准的“视觉问答”。

---

## 📦 项目结构

```text
MemoryLens/
├── README.md              # 项目说明文档 (本文件)
├── ONE_PAGER.md           # 产品概念单页
├── assets/
│   ├── prompts_idea.png   # AI 生成的创意发散图
│   ├── concept_art.png    # Midjourney 生成的产品外观/UI
│   └── market_analysis.png# AI 总结的市场分析报告
├── src/
│   └── demo.py            # 核心视频流处理逻辑 Demo
└── docs/
    └── technical_spec.pdf # 技术规格说明书
```

---

## 🚀 快速开始

### 环境要求
- Python 3.8+
- GPU 支持 (用于本地 SLM 推理)
- SiliconFlow / OpenAI SDK

安装依赖：
```bash
pip install openai
```

### 配置 API Key
设置环境变量（Windows PowerShell）：
```bash
$env:SILICONFLOW_API_KEY="your-api-key-here"
```

或者使用命令行临时设置：
```bash
set SILICONFLOW_API_KEY=your-api-key-here
```

### 运行代码 Demo
```bash
python src/demo.py
```

如果没有设置 API Key，程序会自动使用模拟模式运行。
💡 提示: 若未配置 API Key，程序将自动进入模拟模式，使用预设视频流演示功能流程。

### 查看 UI 原型
打开 assets/concept_art.png 查看由 Midjourney v6 生成的产品概念图与 UI 界面。

---

## 📋 交付物清单

根据 **AI 项目创意征集令** 的要求，本项目包含以下交付物：

1. ✅ **产品概念单页** (`ONE_PAGER.md`)
   - 产品名称、MemoryLens
   - 详细的用户痛点分析 (安全/记忆/情感)
   - 解决方案架构图
   - 商业模式简述

2. ✅ **可视化原型** (`assets/concept_art.png`)
   - 100% AI 生成的产品外观渲染图
   - 交互式 UI 界面设计稿

3. ✅ **代码 Demo** (`src/demo.py`)
   - 由 Cursor/Copilot 辅助生成的核心逻辑
   - 演示视频流分析与 RAG 检索流程

4. ✅ **导师招募画像** (`assets/market_analysis.png`)
   - AI 联网搜索生成的市场规模测算
   - 竞品差异化分析

---

## 🤖 AI 参与度

| 环节 | AI 参与程度 | 工具/方法
|------|------------|
| 创意发散 | 100% |  Prompt 生成 20+ 场景并筛选
| 视觉设计 | 100% |  Midjourney v6 生成概念图/UI
| 功能设计 | 80% |
| UI 设计 | 100% |
| 代码框架 | 80% |  Cursor/Copilot 生成核心逻辑
| 文档撰写 | 70% |  AI 辅助润色与结构化



## 👥 团队

- **创意与设计**: AI + 人类协同
- **代码开发**: AI + 人类调试
- **文档撰写**: 人类洞察 + AI 扩展

---

## 📄 许可证

本项目为课程作业/创新竞赛项目。

---

**让科技更有温度，用 MemoryLens 守护每一位独居老人的晚年生活！👵👴🚀**
