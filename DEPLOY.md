# GitHub 部署指南 / GitHub Deployment Guide

## 📦 准备工作 / Prerequisites

确保您已经安装了 Git：
```bash
git --version
```

## 🚀 推送到 GitHub / Push to GitHub

### 1. 初始化 Git 仓库（如果还没有）
```bash
cd /Users/wen/Desktop/修改个人网站/wenxinchen-soc.github.io-main
git init
```

### 2. 添加所有文件
```bash
git add .
```

### 3. 提交更改
```bash
git commit -m "Initial commit: Personal website with photography section"
```

### 4. 连接到 GitHub 仓库
```bash
# 替换 YOUR_USERNAME 为您的 GitHub 用户名
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
```

### 5. 推送到 GitHub
```bash
git branch -M main
git push -u origin main
```

## 🌐 使用 GitHub Pages 部署 / Deploy with GitHub Pages

### 方法一：在 GitHub 网站上设置

1. 进入您的 GitHub 仓库
2. 点击 **Settings** > **Pages**
3. 在 **Source** 下选择 `main` 分支
4. 点击 **Save**
5. 等待几分钟，您的网站将在 `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/` 上线

### 方法二：使用 GitHub Pages 专用仓库

如果您的仓库名为 `YOUR_USERNAME.github.io`，网站将自动部署到 `https://YOUR_USERNAME.github.io/`

## 📝 后续更新 / Future Updates

每次修改后，使用以下命令推送更新：

```bash
git add .
git commit -m "描述您的更改"
git push
```

## ⚠️ 注意事项 / Notes

- 确保 `.gitignore` 文件已正确配置
- 不要上传敏感信息（API密钥、密码等）
- 图片文件较大时，考虑使用图床或压缩图片
- GitHub Pages 有 1GB 的仓库大小限制

## 🔗 自定义域名（可选）/ Custom Domain (Optional)

如果您有自己的域名：

1. 在仓库根目录创建 `CNAME` 文件
2. 文件内容为您的域名，例如：`www.yourname.com`
3. 在域名提供商处配置 DNS 记录指向 GitHub Pages

---

**需要帮助？** 查看 [GitHub Pages 官方文档](https://docs.github.com/en/pages)
