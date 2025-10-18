# GitHub Pages 部署指南

## 准备工作

确保您已经在GitHub上创建了名为`fortunate`的仓库。

## 部署步骤

### 1. 克隆您的GitHub仓库

```bash
git clone https://github.com/yourusername/fortunate.git
cd fortunate
```

### 2. 将项目文件复制到仓库目录

将以下文件复制到`fortunate`目录中：
- index.html
- style.css
- README.md
- DEPLOY.md (本文件)

### 3. 提交代码

```bash
git add .
git commit -m "Initial deployment of Fortunate student union website"
```

### 4. 推送到GitHub

```bash
git push origin main
```

### 5. 启用GitHub Pages

1. 访问您的GitHub仓库页面：`https://github.com/yourusername/fortunate`
2. 点击顶部的"Settings"选项卡
3. 在左侧导航栏中找到并点击"Pages"
4. 在"Build and deployment"部分，确保"Source"设置为：
   - Source: "Deploy from a branch"
   - Branch: "main" (或您使用的主分支名称)
   - Folder: "/" (根目录)
5. 点击"Save"按钮

### 6. 等待部署完成

GitHub Pages需要几分钟时间来构建和部署您的网站。

### 7. 访问您的网站

部署完成后，您的网站将在以下URL可用：
`https://yourusername.github.io/fortunate/`

## 验证CSS文件是否正确加载

1. 访问您部署的网站
2. 右键点击页面，选择"检查"或"Inspect"
3. 在开发者工具中，切换到"Network"标签
4. 刷新页面
5. 在筛选器中输入"style.css"
6. 确认状态码为200，表示文件已成功加载

## 常见问题解决

### CSS文件未加载

如果CSS文件未正确加载，请检查：

1. **文件路径是否正确**：确保HTML中的链接是`<link rel="stylesheet" href="style.css"/>`
2. **文件是否已提交**：运行`git status`确认style.css已被提交
3. **部署是否完成**：等待几分钟，GitHub Pages部署可能需要时间
4. **浏览器缓存**：尝试使用Ctrl+Shift+R (Windows/Linux)或Cmd+Shift+R (Mac)强制刷新

### 图片资源问题

如果图片无法显示：
1. 确保所有图片使用绝对URL或正确的相对路径
2. 如果使用本地图片，请确保它们已被添加到仓库并提交

## 自动部署

每次您推送到main分支时，GitHub Pages都会自动更新您的网站。

## 自定义域名（可选）

如果您有自定义域名，可以在GitHub Pages设置中配置：
1. 在"Custom domain"字段中输入您的域名
2. 按照指示在您的DNS提供商处添加必要的记录
