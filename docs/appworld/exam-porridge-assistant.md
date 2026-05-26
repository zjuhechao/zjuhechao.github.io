# 考试粥助手

> 一款基于 AI 的本地化学习与考试辅助工具。
>
> 上传学习资料，AI 自动生成复习纲要、学习笔记和练习题，支持刷题、错题追踪和针对性训练。
>
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

### 第一步：安装 Git

Git 是一个代码管理工具，用来把项目从 GitHub 下载到你的电脑上。

<details>
<summary><b>Windows</b>（点击展开）</summary>

<ol>
<li>打开浏览器，访问 https://git-scm.com/downloads</li>
<li>点击 <strong>Windows</strong> 版本下载（会自动下载一个 <code>.exe</code> 安装文件）</li>
<li>双击安装文件，<strong>一路点 Next</strong>，所有选项保持默认即可</li>
<li>安装完成后点击 <strong>Finish</strong></li>
</ol>

</details>

<details>
<summary><b>macOS</b>（点击展开）</summary>

<ol>
<li>打开终端（按 <code>Cmd + 空格</code> 搜索"终端"）</li>
<li>
<p>安装 <a href="https://brew.sh/">Homebrew</a>（若已安装可跳过）：</p>
<pre><code>/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
</code></pre>
</li>
<li>
<p>通过 Homebrew 安装 Git：</p>
<pre><code>brew install git
</code></pre>
</li>
</ol>

</details>

<details>
<summary><b>Linux（以 Ubuntu 为例）</b>（点击展开）</summary>

<ol>
<li>打开终端（<code>Ctrl + Alt + T</code>）</li>
<li>
<p>更新软件包列表并安装 Git：</p>
<pre><code>sudo apt update
sudo apt install git -y
</code></pre>
</li>
</ol>
<p>其他发行版：Fedora 使用 <code>sudo dnf install git</code>，Arch Linux 使用 <code>sudo pacman -S git</code>。</p>

</details>

**验证安装：** 在终端中输入：

```
git --version
```

看到类似 `git version 2.xx.x` 的输出即安装成功。

### 第二步：安装 Node.js

Node.js 是运行本项目所必需的 JavaScript 运行时。

<details>
<summary><b>Windows</b>（点击展开）</summary>

<ol>
<li>打开浏览器，访问 https://nodejs.org/zh-cn</li>
<li>点击 <strong>LTS（长期支持版）</strong> 下载按钮</li>
<li>双击下载好的 <code>.msi</code> 安装文件，一路点 <strong>Next</strong></li>
<li>如果看到 "Automatically install the necessary tools" 选项，<strong>勾选它</strong></li>
<li>点击 <strong>Install</strong>，等待安装完成，点击 <strong>Finish</strong></li>
</ol>

</details>

<details>
<summary><b>macOS</b>（点击展开）</summary>

<p><strong>方法一（推荐）：使用 Homebrew</strong></p>
<pre><code>brew install node
</code></pre>

<p><strong>方法二：从官网下载</strong></p>
<ol>
<li>打开浏览器，访问 https://nodejs.org/zh-cn</li>
<li>点击 <strong>LTS（长期支持版）</strong> 下载按钮</li>
<li>双击下载好的 <code>.pkg</code> 安装文件，按提示完成安装</li>
</ol>

</details>

<details>
<summary><b>Linux（以 Ubuntu 为例）</b>（点击展开）</summary>

<pre><code>sudo apt update
sudo apt install nodejs npm -y
</code></pre>

<blockquote>
<p>如需最新版本，建议使用 <a href="https://github.com/nvm-sh/nvm">nvm</a> 安装：</p>
<pre><code>curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash
# 重启终端后
nvm install --lts
</code></pre>
</blockquote>

</details>

**验证安装：** 在终端中输入：

```
node --version
npm --version
```

看到类似 `v20.11.0` 和 `10.2.4` 的版本号即成功。

### 第三步：下载项目代码

打开终端，进入你希望存放项目的目录，然后运行：

```
git clone https://github.com/zjuhechao/exam-porridge-assistant.git
cd exam-porridge-assistant
```

### 第四步：安装项目依赖

```
npm install
```

> 首次安装需要下载约 200MB 的依赖包，耗时 2-5 分钟。出现黄色的 `WARN` 警告是正常的。
>
> **如果安装很慢或失败：** 切换到国内镜像源后重试：
> ```
> npm config set registry https://registry.npmmirror.com
> npm install
> ```

### 第五步：启动项目

```
npm run dev
```

等待几秒钟，当终端显示 `webpack compiled successfully` 时，说明启动成功。

> 启动后这个终端窗口不要关闭，关闭终端即关闭应用。

### 第六步：打开应用

打开浏览器，在地址栏输入：

```
http://localhost:3015
```

按回车，即可看到考试粥助手的首页。

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

## 🔗 链接

<div class="grid cards" markdown>

-   __GitHub 仓库__

    ---

    浏览完整源码、提交 Issue 或 Star 支持。

    [前往仓库 →](https://github.com/zjuhechao/exam-porridge-assistant){ .md-button .md-button--primary }

</div>
