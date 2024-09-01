# 创建一个 Hugo 网站的步骤

创建一个 Hugo 网站的步骤如下，确保你有基本的开发环境准备好（如 Git 和 Go 环境），并且已经安装好 Hugo。如果还未安装 Hugo，你可以参考 [Hugo 官方安装文档](https://gohugo.io/getting-started/installing/) 进行安装。



## 1. 安装 Hugo


如果尚未安装 Hugo，可以按照以下步骤安装：

- **MacOS (使用 Homebrew):**
  ```bash
  brew install hugo
  ```
  
- **Windows (使用 Chocolatey):**
  ```bash
  choco install hugo -confirm
  ```

- **Linux (使用 apt):**
  ```bash
  sudo apt-get install hugo
  ```

## 2. 创建网站项目
使用 [hugoplate](https://github.com/zeon-studio/hugoplate) 作为项目模版， 通过 `Use this template` and `Create a new repository`

使用 Hugo 命令行工具创建一个新的项目：

```bash
git clone https://github.com/crazynomad/weneedtowin
```

将 `weneedtowin` 替换为你的网站名称。这个命令会生成一个包含 Hugo 项目所需文件和文件夹的目录结构。

## 🚀 Getting Started

First you need to [clone](https://github.com/zeon-studio/hugoplate) or [download](https://github.com/zeon-studio/hugoplate/archive/refs/heads/main.zip) the template repository, and then let's get started with the following process:

### ⚙️ Prerequisites

To start using this template, you need to have some prerequisites installed on your machine.

- [Hugo Extended v0.124+](https://gohugo.io/installation/)
- [Node v20+](https://nodejs.org/en/download/)
- [Go v1.22+](https://go.dev/doc/install)

### 👉 Project Setup

We build this custom script to make your project setup easier. It will create a new Hugo theme folder, and clone the Hugoplate theme into it. Then move the exampleSite folder into the root directory. So that you can start your Hugo server without going into the exampleSite folder. Use the following command to setup your project.

```bash
npm run project-setup
```

### 👉 Install Dependencies

Install all the dependencies using the following command.

```bash
npm install
```

### 👉 Development Command

Start the development server using the following command.

```bash
npm run dev
```

### 🎬 Still Confused? Watch a Quick Video

https://github.com/zeon-studio/hugoplate/assets/58769763/c260c0ae-91be-42ce-b8db-aa7f11f777bd

---

## 3. 创建内容

使用 Hugo 创建页面和文章。例如，创建首页内容：

```bash
hugo new _index.md
```

创建服务页面：

```bash
hugo new services.md
```

Hugo 会在 `content` 文件夹中生成对应的 Markdown 文件，可以编辑这些文件并添加页面内容。

## 6. **启动本地服务器**

启动 Hugo 本地开发服务器以查看实时的开发效果：

```bash
hugo server -D
```

访问 [http://localhost:1313](http://localhost:1313) 可以看到你正在开发的网站。

## 7. **自定义设计**

在 `themes/hugo-coder/layouts` 或 `layouts` 目录中编辑模板文件，修改 HTML 和样式，使其符合你的设计需求。

## 8. **生成静态网站**

开发完成后，生成静态文件以供发布：

```bash
hugo
```

生成的静态文件会位于 `public` 文件夹中，你可以将这些文件部署到任意支持静态文件的网站托管服务（如 GitHub Pages、Netlify、Vercel 等）。

## 9. **部署网站**

将 `public` 文件夹中的内容上传到你选择的托管平台。常见的 Hugo 部署方式有：


- **GitHub Pages**：将生成的 `public` 文件夹推送到 GitHub 仓库的 `gh-pages` 分支。
- **Netlify**：连接 GitHub 仓库并选择自动构建和部署。
- **Vercel**：导入 GitHub 项目并配置 Hugo 的部署设置。

### 总结

这些步骤将帮助你从零开始搭建一个 Hugo 网站，并进行本地开发、配置主题、创建内容、生成静态文件以及部署上线。如果需要任何特定部分的详细讲解或定制化配置，请告诉我！