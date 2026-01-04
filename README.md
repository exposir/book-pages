# 深度阅读档案馆

这是一个书籍与思想深度分析网页项目，通过 GitHub Pages 部署为独立的在线阅读页面。

## 在线访问

🌐 **项目主页：** https://exposir.github.io/book-pages/

### 页面列表

#### 红色赌盘系列

- **章节详细版**：[red-roulette-chapters.html](https://exposir.github.io/book-pages/red-roulette-chapters.html)
  多章节导航式深度解析，包含：封面、核心人物、温家宝专题、平安保险案、机场物流案、编年史、结局等独立页面

- **时间线分析版**：[red-roulette-timeline.html](https://exposir.github.io/book-pages/red-roulette-timeline.html)
  可视化分析版本，包含：关系网图（Mermaid）、全景时间线、剧情解析、任务链等分析工具

#### 思想史系列

- **八种社会思潮档案**：[eight-thoughts-archive.html](https://exposir.github.io/book-pages/eight-thoughts-archive.html)
  当代中国八种社会思潮深度全景档案，包含：历史编年、思潮分析、关键事件、代表人物等内容

## 项目特点

- ✅ **零依赖部署** - 所有依赖通过 CDN 加载，无需 npm 或构建工具
- ✅ **自包含设计** - 每个 HTML 文件都是独立完整的应用
- ✅ **现代技术栈** - 使用 React + Tailwind CSS + Mermaid.js
- ✅ **响应式设计** - 适配桌面和移动设备
- ✅ **中文优化** - 针对中文内容优化排版和阅读体验

## 技术架构

每个页面都是完整的单页应用：
- React 18 (UMD) - 通过 unpkg.com 加载
- Babel Standalone - 浏览器端 JSX 编译
- Tailwind CSS - CDN 方式引入
- Mermaid.js - 用于关系图可视化

## 更新内容

如需添加或修改内容，只需编辑对应的 HTML 文件后推送：

```bash
git add .
git commit -m "更新内容"
git push
```

GitHub Pages 会在 1-2 分钟内自动更新。

## 开发说明

详细的开发指南请参考 [CLAUDE.md](CLAUDE.md)。

## License

本项目用于学术研究和教育目的。内容基于《红色赌盘》一书的公开信息整理。
