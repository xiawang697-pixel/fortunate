# Fortunate 学生会竞选网站

这是一个现代化的学生会竞选宣传网站，包含互动功能和梦幻特效，专为GitHub Pages部署优化。

## 功能特点

- 响应式设计，适配各种设备
- 互动按钮与点击计数系统
- 梦幻特效（粒子、光尾、星星等）
- 平滑滚动和动画效果
- 完整的竞选信息展示

## GitHub Pages 部署指南

### 1. 准备工作

确保你的项目结构如下结构：
```
student_union_website/
├── index.html
├── style.css
└── README.md
```

### 2. 创建创建GitHub仓库

1. 登录GitHub，创建一个新的仓库，命名为 `fortunate`
2. 在本地计算机上，将项目文件夹重命名为 `fortunate`

### 3. 初始化Git仓库

```bash
# 进入项目目录
cd /path/to/fortunate

# 初始化Git仓库
git init

# 添加所有文件
git add .

# 提交更改
git commit -m "Initial commit"
```

### 4. 连接GitHub仓库

```bash
# 添加远程仓库
git remote add origin https://github.com/xiawang697-pixel/fortunate.git

# 推送到本地分支重命名为main（GitHub默认分支）
git branch -M main

# 推送代码到GitHub
git push -u origin main
```

### 5. 启用GitHub Pages

1. 进入GitHub仓库页面
2. 点击右上角的 "Settings"
3. 在左侧菜单中选择 "Pages"
4. 在 "Source" 部分，选择分支为 "main"，文件夹为 "/"
5. 点击 "Save"
6. 等待几分钟，你的网站将部署在：`https://xiawang697-pixel.github.io/fortunate/`

### 6. 验证部署

1. 访问你的网站地址：`https://xiawang697-pixel.github.io/fortunate/`
2. 检查所有样式和交互功能是否正常工作
3. 点击右下角的互动按钮，验证动画效果是否正常

### 7. 后续更新

当你需要更新网站时，只需：

```bash
# 添加更改
git add .

# 提交更改
git commit -m "Update description"

# 推送更新
git push
```

GitHub Pages将自动重新部署你的网站。

### 常见问题解决

1. **CSS不加载**：
   - 确保`style.css`文件在根目录
   - 检查HTML中的引用路径是否正确：`<link rel="stylesheet" href="style.css">`
   - 清除浏览器缓存后重试

2. **图片不显示**：
   - 确保图片路径正确
   - 对于GitHub Pages，建议使用相对路径

3. **互动功能不工作**：
   - 检查浏览器控制台是否有JavaScript错误
   - 确保所有脚本都在HTML中正确引用

## 联系方式

如有任何问题，请联系我们的开发团队。
