# YouTube-Style Bilibili Frontend

<p align="center">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white" alt="CSS3">
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black" alt="JavaScript">
  <img src="https://img.shields.io/badge/Bilibili_API-00A1D6?style=flat&logo=bilibili&logoColor=white" alt="Bilibili">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License">
</p>

<p align="center">
  <b>一个仿 YouTube 界面的 Bilibili 视频浏览前端应用</b><br>
  <i>纯前端实现 · 响应式设计 · 实时搜索 · 视频播放</i>
</p>

---

## ✨ 功能特性

- 🎨 **YouTube 风格界面** — 高度还原 YouTube 的现代化 UI 设计
- 🔍 **实时视频搜索** — 通过 Bilibili API 搜索真实视频内容
- 📺 **嵌入式播放** — 集成 Bilibili 官方播放器，支持高清播放
- 📱 **响应式布局** — 完美适配桌面端、平板和移动设备
- 🏠 **智能首页** — 自动加载热门视频，支持分类筛选
- 💾 **离线缓存** — 网络异常时自动切换本地备用数据
- 🌐 **CORS 代理支持** — 内置多个代理源，提高 API 可用性

---

## 🚀 快速开始

### 在线预览

直接在浏览器中打开 `index.html` 即可运行，无需构建工具。

```bash
# 克隆仓库
git clone https://github.com/yourusername/youtube-bilibili-frontend.git

# 进入目录
cd youtube-bilibili-frontend

# 打开项目（任选其一）
open index.html              # macOS
start index.html             # Windows
python -m http.server 8080   # 本地服务器
```

---

## 📁 项目结构

```
youtube-bilibili-frontend/
├── index.html          # 主页面（单文件应用）
├── README.md           # 项目说明
└── LICENSE             # MIT 许可证
```

> **注意**：本项目为单文件应用，所有 HTML、CSS、JavaScript 均集成在 `index.html` 中，便于快速部署。

---

## 🛠️ 技术栈

| 技术 | 说明 |
|------|------|
| **HTML5** | 语义化标签，支持视频嵌入 |
| **CSS3** | Flexbox/Grid 布局，CSS 变量，响应式设计 |
| **Vanilla JS** | 原生 JavaScript，无框架依赖 |
| **Bilibili API** | 搜索接口、视频信息获取 |
| **Font Awesome** | 图标库（CDN 引入） |
| **Google Fonts** | Roboto 字体（CDN 引入） |

---

## 🔌 API 说明

本项目使用 Bilibili 公开 API 获取数据：

| 接口 | 用途 | 示例 |
|------|------|------|
| `x/web-interface/search/type` | 视频搜索 | 关键词搜索、分类筛选 |
| `player.bilibili.com` | 视频播放 | 嵌入 iframe 播放器 |

### CORS 代理

由于浏览器跨域限制，项目内置了以下代理服务：
- `allorigins.win`
- `codetabs.com`

> 代理服务可能因网络环境不稳定，项目会自动降级到本地缓存数据。

---

## 📱 响应式断点

| 断点 | 布局调整 |
|------|----------|
| `> 1200px` | 视频播放页双栏布局（播放器 + 推荐列表） |
| `768px - 1200px` | 单栏布局，隐藏侧边推荐 |
| `< 768px` | 移动端布局，单列视频网格，隐藏侧边栏 |

---

## 🎯 使用指南

### 搜索视频
1. 在顶部搜索框输入关键词（如："科技"、"美食"）
2. 按 `Enter` 或点击搜索按钮
3. 系统自动调用 Bilibili API 返回搜索结果

### 播放视频
1. 点击任意视频卡片
2. 页面切换至播放界面
3. 右侧显示相关推荐视频

### 分类筛选
- 首页顶部提供分类标签（游戏、音乐、科技、美食等）
- 点击标签快速筛选对应类型视频

---

## ⚠️ 免责声明

本项目仅供学习交流使用：
- 所有视频内容版权归 [Bilibili](https://www.bilibili.com) 及其 UP 主所有
- 界面设计参考 [YouTube](https://www.youtube.com) 仅供学习目的
- 请勿用于商业用途

---

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建功能分支：`git checkout -b feature/AmazingFeature`
3. 提交更改：`git commit -m 'Add some AmazingFeature'`
4. 推送分支：`git push origin feature/AmazingFeature`
5. 提交 Pull Request

---

## 📄 许可证

本项目采用 [MIT License](LICENSE) 开源许可证。

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/yourusername">Your Name</a>
</p>
