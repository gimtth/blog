# 时光褶皱 - 个人博客网站

<div align="center">
  <img src="./image.png" alt="项目预览" width="800">
  
  [![GitHub license](https://img.shields.io/badge/license-MulanPSL--2.0-blue.svg)](LICENSE)
  [![GitHub stars](https://img.shields.io/github/stars/gimtth/blog?style=social)](https://github.com/gimtth/blog/stargazers)
  [![GitHub forks](https://img.shields.io/github/forks/gimtth/blog?style=social)](https://github.com/gimtth/blog/network/members)
  [![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
  [![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
  [![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
  
  一个简洁优雅的个人博客网站，包含项目展示、个人简历、博客文章、书签导航等功能。
</div>

---

## ✨ 特性

- 🎨 **现代化设计** - 简洁优雅的 UI 设计，支持深色/浅色主题切换
- 📱 **响应式布局** - 完美适配桌面端、平板和移动设备
- 🎭 **动态背景** - Canvas 动画背景，提升视觉体验
- 📝 **Markdown 支持** - 博客文章支持 Markdown 格式编写
- 🔖 **书签导航** - 27个分类，190+精选网站书签
- 💼 **项目展示** - 专业的项目作品展示页面
- 📄 **在线简历** - 交互式个人简历页面
- 🌐 **SEO 优化** - 良好的搜索引擎优化

## 🎯 页面功能

| 页面 | 文件 | 功能描述 |
|------|------|---------|
| 🏠 主页 | `index.html` | 网站首页，展示个人信息和导航 |
| 💼 项目 | `home.html` | 项目作品集展示 |
| 📋 经验 | `resume.html` | 个人简历与工作经历 |
| 📧 联系 | `contact.html` | 联系方式与社交媒体 |
| ✍️ 博客 | `blog.html` | 文章列表与博客管理 |
| 🔖 书签 | `bookmark.html` | 27个分类的精选网站导航 |
| 🎬 其他 | `live.html` | 视频直播或其他内容 |

## 🚀 快速开始

### 环境要求

- 现代化浏览器（Chrome、Firefox、Safari、Edge 等）
- 本地服务器（可选，用于开发）

### 安装步骤

1. **克隆项目**
   ```bash
   git clone https://github.com/gimtth/blog.git
   cd blog
   ```

2. **启动项目**
   
   方式一：直接打开（推荐用于快速预览）
   ```bash
   # 直接在浏览器中打开 index.html
   open index.html  # macOS
   start index.html # Windows
   ```
   
   方式二：使用本地服务器（推荐用于开发）
   ```bash
   # 使用 Python
   python -m http.server 8080
   
   # 使用 Node.js (需要先安装 http-server)
   npx http-server -p 8080
   
   # 使用 PHP
   php -S localhost:8080
   ```

3. **访问网站**
   
   在浏览器中打开：`http://localhost:8080`

## 📁 项目结构

```
blog/
├── index.html              # 网站主页
├── home.html              # 项目展示页
├── resume.html            # 个人简历页
├── contact.html           # 联系方式页
├── blog.html              # 博客列表页
├── bookmark.html          # 书签导航页
├── live.html              # 其他内容页
├── showmd.html            # Markdown 文章展示页
│
├── css/                   # 样式文件
│   ├── base.css          # 基础样式和主题
│   ├── home.css          # 主页样式
│   ├── index1.css        # 通用组件样式
│   ├── blog.css          # 博客页样式
│   ├── resume.css        # 简历页样式
│   ├── contact.css       # 联系页样式
│   ├── live.css          # 其他页面样式
│   └── ...               # 其他样式文件
│
├── js/                    # JavaScript 文件
│   ├── base.js           # 基础功能（主题切换等）
│   ├── canvas.js         # Canvas 动画背景
│   ├── jquery.min.js     # jQuery 库
│   ├── marked.js         # Markdown 解析器
│   ├── prism.js          # 代码高亮
│   └── ...               # 其他 JS 文件
│
├── img/                   # 图片资源
│   ├── back/             # 背景图片
│   ├── project/          # 项目截图
│   └── ...               # 其他图片
│
├── LICENSE               # 开源协议
└── README.md            # 项目说明文档
```

## 🎨 主题定制

网站支持深色/浅色主题切换，点击右上角的主题切换按钮即可。

### 自定义主题颜色

在 `css/base.css` 中修改 CSS 变量：

```css
:root {
  --mainColor: #2c3e50;        /* 主要文字颜色 */
  --bgColor: #ffffff;          /* 背景颜色 */
  --headerFont: #2c3e50;       /* 标题颜色 */
  --pColor: #7f8c8d;          /* 段落文字颜色 */
  /* ... 更多颜色变量 */
}

[data-theme='dark'] {
  --mainColor: #ecf0f1;
  --bgColor: #1a1a1a;
  /* ... 深色主题颜色 */
}
```

## 📚 书签导航

书签页面包含 **27个精选分类**，涵盖 **190+** 优质网站：

- 🤖 AI工具 - AI开发、设计、对话等
- 🛠️ 开发工具 - Git、IDE、在线工具
- 📚 学习资源 - 网课、教程、文档
- 🎨 设计素材 - 图片、视频、音频、字体
- 💼 办公模板 - PPT、文档模板
- 🎮 娱乐休闲 - 影视、音乐、游戏
- 📱 更多分类...

每个书签卡片都经过精心设计，每行显示3个，布局整齐美观。

## 🔧 技术栈

### 前端技术
- **HTML5** - 语义化标签，SEO 优化
- **CSS3** - Flexbox、Grid 布局，CSS 变量
- **JavaScript** - 原生 JS + jQuery
- **Canvas** - 动态背景动画

### 第三方库
- **jQuery** - DOM 操作和事件处理
- **Marked.js** - Markdown 解析
- **Prism.js** - 代码语法高亮
- **Paper.js** - Canvas 图形库
- **Font Awesome** - 图标库

## 📝 如何使用

### 添加博客文章

1. 创建 Markdown 文件（`.md` 格式）
2. 在 `blog.html` 中添加文章链接
3. 文章会通过 `showmd.html` 页面展示

示例：
```markdown
# 文章标题

这是文章内容...

## 二级标题

更多内容...
```

### 添加项目展示

在 `home.html` 中的项目列表部分添加新项目：

```html
<div class="li1-box-item">
  <img src="./img/project/your-project.png" alt="项目名称">
  <div class="boxitem-title">
    <h6>项目名称</h6>
    <p>项目简介</p>
  </div>
</div>
```

### 添加书签

在 `bookmark.html` 中添加新的书签卡片：

```html
<div class="carbox">
  <div class="li6car-title">
    <h4>网站名称</h4>
    <p>网站描述</p>
    <div class="borderbotm"></div>
    <a href="网站链接" target="_blank">访问网站</a>
  </div>
</div>
```

## 🎯 浏览器兼容性

| 浏览器 | 版本 |
|--------|------|
| Chrome | ✅ 最新版 |
| Firefox | ✅ 最新版 |
| Safari | ✅ 最新版 |
| Edge | ✅ 最新版 |
| IE | ❌ 不支持 |

## 📸 页面预览

### 主页
干净简洁的首页设计，动态 Canvas 背景

### 项目页
网格布局展示项目作品集

### 博客页
文章列表与 Markdown 文章展示

### 书签页
27个分类，190+精选网站，每行3个卡片

## 🤝 贡献

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建你的特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交你的改动 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启一个 Pull Request

## 📄 开源协议

本项目采用 MulanPSL-2.0 协议 - 查看 [LICENSE](LICENSE) 文件了解详情

## 👨‍💻 作者

**时光褶皱**

- 个人网站：[https://gimtth.github.io/blog](https://gimtth.github.io/blog)
- GitHub：[@gimtth](https://github.com/gimtth)
- Email：你的邮箱

## 🙏 致谢

- 感谢所有开源库的作者
- 感谢所有为项目做出贡献的开发者

## 📮 联系方式

如有问题或建议，欢迎通过以下方式联系：

- 📧 Email：你的邮箱
- 💬 GitHub Issues：[提交问题](https://github.com/gimtth/blog/issues)

---

<div align="center">
  
  **⭐ 如果这个项目对你有帮助，请给一个 Star ⭐**
  
  Made with ❤️ by 时光褶皱
  
</div>

