# 考试粥助手

<div class="grid cards" markdown>

-   :material-brain: **AI 驱动**

    自动生成复习纲要、学习笔记和练习题

-   :material-database-off: **数据全本地**

    所有数据在浏览器本地，无需服务器

-   :material-github: **开源免费**

    代码完全开放，自行配置 API Key 即可使用

</div>

---

## 简介

**考试粥助手** 是一个 AI 驱动的智能备考工具。上传你的学习资料（PDF / Word / TXT / 图片），AI 自动帮你整理知识、生成复习提纲和学习笔记、出题练习，搭配错题本实现高效复习闭环。

---

## 核心功能

<div class="grid" markdown>

<div markdown>

:material-file-document-outline:{ .lg .middle } **知识库管理**

上传多种格式的学习资料，AI 自动提取文本，按课程分类管理。

</div>
<div markdown>

:material-book-search-outline:{ .lg .middle } **复习纲要 & 学习笔记**

AI 根据文档内容自动生成结构化复习纲要和详细笔记，涵盖知识点归纳与重点解析。

</div>
<div markdown>

:material-head-question-outline:{ .lg .middle } **智能出题**

支持选择题、填空题、判断题、简答题，难度可调，AI 根据学习内容自动出题。

</div>
<div markdown>

:material-close-circle-outline:{ .lg .middle } **错题本**

自动收集错题，标记掌握程度，支持基于错题重新出题强化。

</div>
<div markdown>

:material-file-upload-outline:{ .lg .middle } **刷题器 & OCR**

导入已有试卷，AI 自动识别题目结构并补全答案。支持图片 OCR 识别纸质资料。

</div>
<div markdown>

:material-shield-lock-outline:{ .lg .middle } **隐私安全**

所有数据存储在浏览器本地，不经过任何服务器。仅 AI 调用需要联网。

</div>
</div>

---

## 快速上手

### 1. 获取项目

```bash
git clone https://github.com/zjuhechao/exam-porridge-assistant.git
cd exam-porridge-assistant
npm install
npm run dev
```

或者直接从 [Release 页面](https://github.com/zjuhechao/exam-porridge-assistant/releases) 下载构建好的版本。

### 2. 配置 API

打开设置页面，填写你的 AI API 信息：

| 配置项 | 说明 | 示例 |
|:---|:---|:---|
| API Base URL | API 服务地址 | `https://api.deepseek.com` |
| API Key | 你的密钥 | `sk-...` |
| 模型名称 | 使用的模型 | `deepseek-chat` |

支持 DeepSeek / OpenAI / Claude 等所有兼容 OpenAI 格式的 API。

### 3. 开始使用

1. 创建课程，上传学习资料
2. 使用"复习助手"生成纲要和笔记
3. 在"智能答题"中选择文档和题型进行练习
4. 错题自动收入错题本，针对性巩固

---

## 技术特点

- **纯前端**：React + TypeScript + Webpack + Tailwind CSS
- **本地存储**：IndexedDB (Dexie) + localStorage，无需后端
- **学科定制**：按数学、物理、化学、计算机等学科定制 AI 提示词
- **多 API 支持**：可为不同功能分配不同的 API 配置

---

## 链接

<div class="grid cards" markdown>

-   [**:simple-github: GitHub 仓库**](https://github.com/zjuhechao/exam-porridge-assistant){ .md-button .md-button--primary }
-   [**:material-tag: 发布列表**](https://github.com/zjuhechao/exam-porridge-assistant/releases){ .md-button }
-   [**:material-account: 作者主页**](https://github.com/zjuhechao){ .md-button }

</div>
