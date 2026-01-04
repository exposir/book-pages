# 书籍网页项目

这是一个简单的HTML书籍网页项目，可以通过GitHub Pages部署。

## 文件结构

- `index.html` - 主页/目录页
- `chapter1.html` - 第一章
- `chapter2.html` - 第二章
- `chapter3.html` - 第三章

你可以继续添加更多的HTML文件。

## 如何部署到GitHub Pages

1. 在GitHub上创建一个新仓库
2. 将这个文件夹的内容推送到仓库：
   ```bash
   cd book-pages
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/你的用户名/你的仓库名.git
   git push -u origin main
   ```

3. 在GitHub仓库设置中启用GitHub Pages：
   - 进入仓库的 Settings > Pages
   - 在 "Source" 下选择 "main" 分支
   - 点击 Save

4. 访问你的网页：
   - 主页：`https://你的用户名.github.io/你的仓库名/`
   - 各章节：`https://你的用户名.github.io/你的仓库名/chapter1.html`

## 注意事项

- 每个HTML文件都会有独立的URL
- 确保文件名使用小写字母和连字符，避免空格
- GitHub Pages可能需要几分钟才能生效
