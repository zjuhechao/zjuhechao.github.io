# 考试粥助手

> 一款基于 AI 的本地化学习与考试辅助工具。上传学习资料，AI 自动生成复习纲要、学习笔记和练习题，支持刷题、错题追踪和针对性训练。  
> 所有数据完全存储在本地浏览器中，不依赖任何云端服务。

---

## 📋 功能一览

- **多格式资料上传**：支持 PDF、DOCX、TXT、图片等格式，自动提取文本或 OCR 识别
- **AI 复习纲要**：智能生成结构化复习纲要和学习笔记
- **智能出题**：自动生成选择题、填空题、判断题、简答题
- **刷题器模式**：导入已有题目文件或试卷图片，AI 自动识别题目
- **错题追踪**：自动收集错题，针对性强化训练
- **课程管理**：按课程隔离管理所有学习数据

---

## 🚀 快速上手

### 本地运行

```bash
git clone https://github.com/zjuhechao/exam-porridge-assistant.git
cd exam-porridge-assistant
npm install
npm run dev
```

启动后打开浏览器访问 `http://localhost:3015`。

> GitHub 仓库提供了从零开始的完整教程，覆盖 Windows / macOS / Linux 全平台。

### 配置 AI

应用的核心功能需要 AI API 支持。支持的 AI 服务商：

| 服务商 | 说明 |
|--------|------|
| DeepSeek | 国内直连，价格低 |
| 通义千问 | 有免费额度 |
| OpenAI | 需海外网络 |

在应用内进入"设置"页面，添加 API 配置即可使用。

---

## ⚙️ 技术栈

| 层 | 技术 |
|----|------|
| 前端框架 | React 18 + TypeScript |
| 路由 | react-router-dom v6 |
| 样式 | Tailwind CSS 3 |
| 动画 | framer-motion |
| 本地数据库 | Dexie (IndexedDB) |
| PDF 解析 | pdfjs-dist |
| DOCX 解析 | mammoth |
| 构建工具 | Webpack 5 |
| AI 接口 | OpenAI 兼容格式（支持多模态） |

---

## ❓ 常见问题

<details>
<summary><b>AI 功能不工作？</b></summary>

在设置页面检查 API Key、Base URL 和模型名称是否正确填写，并确保点击了"保存设置"。按 F12 查看控制台是否有具体的错误信息。
</details>

<details>
<summary><b>数据会丢失吗？</b></summary>

所有数据存储在浏览器本地（IndexedDB）。清除浏览器缓存会丢失数据，不同浏览器之间不共享。建议定期用导出功能备份重要内容。
</details>

<details>
<summary><b>如何更新到最新版本？</b></summary>

在项目文件夹中运行：

```
git pull
npm install
npm run dev
```

</details>

---

## 🔗 链接

<div class="grid cards" markdown>

-   [**GitHub 仓库**](https://github.com/zjuhechao/exam-porridge-assistant){ .md-button .md-button--primary }

</div>
