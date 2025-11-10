# 日本十大经典徒步路线地图

一个基于Web的互动地图应用，展示日本最美的十条经典徒步路线。使用Leaflet地图库和现代化的响应式设计，为徒步爱好者提供直观的路线信息和交互体验。

## 🗾 项目特色

- **交互式地图**：基于Leaflet的响应式地图界面
- **路线详情**：每条路线包含详细信息（难度、地区、最佳季节等）
- **视觉化展示**：不同难度等级使用颜色编码（绿色-简单，橙色-中等，红色-困难）
- **响应式设计**：完美适配桌面端、平板和移动设备
- **多重备份**：3个地图图层源，自动切换确保稳定性
- **加载优化**：智能加载状态指示和错误处理机制

## 🏔️ 包含的徒步路线

1. **富士山吉田路线** - 日本象征，适合初级登山者
2. **高尾山** - 东京近郊，交通便利
3. **奥日光** - 华严瀑布与湿原美景
4. **白神山地** - 世界自然遗产
5. **屋久岛** - 苔藓森林与绳文杉
6. **上高地** - 日本阿尔卑斯门户
7. **立山黑部** - 阿尔卑斯山脉路线
8. **阿苏山** - 活火山徒步体验
9. **知床五湖** - 北海道原始森林
10. **大山** - 出云地区的圣山

## 🛠️ 技术栈

- **前端框架**：原生HTML5 + CSS3 + JavaScript (ES6+)
- **UI框架**：Tailwind CSS
- **地图引擎**：Leaflet.js
- **图标库**：Font Awesome
- **构建工具**：无需构建，纯静态文件
- **部署平台**：GitHub Pages

## 🚀 快速开始

### 本地开发

1. **克隆仓库**
   ```bash
   git clone https://github.com/your-username/japan-hiking-routes.git
   cd japan-hiking-routes
   ```

2. **本地运行**
   ```bash
   # 使用Python HTTP服务器
   python3 -m http.server 8000
   
   # 或使用Node.js http-server
   npx http-server -p 8000
   ```

3. **访问应用**
   打开浏览器访问 `http://localhost:8000`

### 直接部署

由于这是一个纯静态项目，您可以直接将文件上传到任何静态托管服务：

- **GitHub Pages**（推荐）
- **Netlify**
- **Vercel**
- **阿里云OSS**
- **腾讯云COS**

## 📱 响应式特性

### 桌面端 (1200px+)
- 地图高度：80vh（最小800px）
- 最大宽度：1400px，居中显示
- 三列路线列表布局

### 平板端 (768px-1200px)
- 地图高度：75vh（最小700px）
- 两列路线列表布局
- 优化的触摸交互

### 移动端 (768px以下)
- 地图高度：70vh（最小500px）
- 单列路线列表布局
- 移动端优化的控制按钮

## 🎨 设计亮点

### 颜色方案
- **主色调**：自然绿 (#2E7D32) - 体现户外徒步主题
- **辅助色**：木色调 (#8D6E63) - 温暖的自然感
- **强调色**：橙色 (#FF8F00) - 活力与冒险
- **背景色**：浅绿色 (#F1F8E9) - 舒适的视觉体验

### 交互设计
- **智能加载**：显示加载动画和错误提示
- **图层备份**：3个地图源自动切换
- **标记优化**：扩大版图标，提高可读性
- **弹出窗口**：详细信息展示，响应式宽度

## 🔧 配置说明

### 地图配置
```javascript
const mapConfig = {
  center: [36.2048, 138.2529], // 日本中心坐标
  zoom: 5, // 初始缩放级别
  tileLayers: [ // 多个图层源
    {
      url: 'https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png',
      attribution: '© OpenStreetMap contributors'
    }
    // ... 更多图层
  ]
};
```

### 路线数据结构
```javascript
const hikingRoutes = [
  {
    id: 1,
    name: "路线名称",
    region: "地区",
    location: "具体位置",
    coordinates: [纬度, 经度],
    difficulty: "难度等级",
    difficultyLevel: "easy|medium|hard",
    season: "最佳季节",
    keywords: "关键词",
    description: "详细描述"
  }
  // ... 更多路线
];
```

## 🌐 浏览器兼容性

- ✅ Chrome 60+
- ✅ Firefox 55+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ 移动端浏览器（iOS Safari, Chrome for Android）

## 🤝 贡献指南

欢迎提交Issue和Pull Request来改进这个项目！

### 提交Issue
- 报告bug时请注明浏览器版本和复现步骤
- 功能建议请详细描述使用场景

### 提交代码
1. Fork 本仓库
2. 创建您的功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个Pull Request

## 📄 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 🙏 致谢

- [Leaflet.js](https://leafletjs.com/) - 优秀的开源地图库
- [OpenStreetMap](https://www.openstreetmap.org/) - 免费地图数据
- [Tailwind CSS](https://tailwindcss.com/) - 实用优先的CSS框架
- [Font Awesome](https://fontawesome.com/) - 图标字体库

## 📞 联系方式

- 项目维护者：[您的姓名]
- 邮箱：[your.email@example.com]
- 项目主页：https://github.com/your-username/japan-hiking-routes

---

⭐ 如果这个项目对您有帮助，请给它一个星标！