# AIVO Support Website

App Store 支持页面 - 多语言支持（中/英/日/韩）

## 📁 项目结构

```
awaken-support/
├── index.html          # 主页（自动检测语言跳转）
├── en/
│   └── index.html      # 英文支持页
├── zh/
│   └── index.html      # 中文支持页
├── ja/
│   └── index.html      # 日文支持页
├── ko/
│   └── index.html      # 韩文支持页
├── privacy.html        # 隐私政策
├── terms.html          # 服务条款
├── css/
│   └── style.css       # 统一样式
└── README.md
```

## 🚀 快速部署到 GitHub Pages

### 步骤 1: 创建 GitHub 仓库

```bash
# 在 GitHub 上创建新仓库：awaken-support
```

### 步骤 2: 初始化并推送

```bash
cd awaken-support
git init
git add .
git commit -m "Initial commit: AIVO support page"
git branch -M main
git remote add origin https://github.com/你的用户名/awaken-support.git
git push -u origin main
```

### 步骤 3: 启用 GitHub Pages

1. 进入仓库 Settings
2. 找到 Pages 选项
3. Source 选择 `main` 分支
4. 保存

### 步骤 4: 获取 URL

部署完成后（约 1-2 分钟），访问：
```
https://你的用户名.github.io/awaken-support/
```

## 🌐 自定义域名（可选）

1. 在根目录创建 `CNAME` 文件：
```
support.yourapp.com
```

2. 在域名服务商添加 DNS 记录：
```
类型: CNAME
主机: support
值: 你的用户名.github.io
```

## 📱 App Store Connect 配置

填写以下 URL：
- **Support URL**: `https://你的用户名.github.io/awaken-support/`
- **Privacy Policy URL**: `https://你的用户名.github.io/awaken-support/privacy.html`

## ✏️ 自定义内容

### 修改联系邮箱

在各语言的 `index.html` 文件中搜索并替换：
- `support@aivo.app` → 你的支持邮箱

### 修改 App 名称

搜索并替换所有 `AIVO` 为你的 App 名称

### 修改版本号

在 footer 部分修改 `Version 1.0.0`

## 🎨 样式定制

编辑 `css/style.css` 中的 CSS 变量：

```css
:root {
  --color-bg: #0a0a0f;           /* 背景色 */
  --color-primary: #6366f1;       /* 主题色 */
  --color-accent: #8b5cf6;        /* 强调色 */
  --color-text: #e4e4e7;          /* 文字色 */
}
```

## 📄 License

MIT License

