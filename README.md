# 健康管理工具 - FatTime

一个专为都市上班族设计的健身记录应用，支持快速记录运动数据、体重追踪和数据分析。

## 🎯 功能特点

- **快速记录**: 5分钟内完成运动数据录入
- **全面追踪**: 运动类型、组数、次数、重量、疲劳度、心情
- **体重管理**: 每日体重记录和趋势分析
- **数据可视化**: 训练频率、体重变化图表
- **离线使用**: PWA支持，数据本地存储
- **移动优化**: 响应式设计，完美适配手机

## 🛠️ 技术栈

- **前端**: Vue 3 + TypeScript + Vite
- **UI组件**: Vant 4 (移动端UI库)
- **状态管理**: Pinia
- **数据存储**: IndexedDB + Dexie.js
- **PWA**: Workbox + Vite PWA Plugin
- **部署**: GitHub Pages

## 🚀 快速开始

### 本地开发

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build

# 预览构建结果
npm run preview
```

### 部署到GitHub Pages

1. **推送到GitHub**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/yourusername/fattime.git
   git push -u origin main
   ```

2. **启用GitHub Pages**:
   - 在GitHub仓库页面，点击 "Settings" 选项卡
   - 在左侧菜单中找到 "Pages"
   - Source: 选择 "GitHub Actions"
   - 推送代码后自动构建和部署
   - 访问链接: `https://yourusername.github.io/fattime`

## 📱 使用指南

### 运动记录
1. 点击"开始记录"进入记录页面
2. 选择运动类型或添加自定义运动
3. 输入组数、次数、重量
4. 记录疲劳度(1-5级)和心情(1-5级)
5. 可选记录当日体重
6. 保存记录

### 数据查看
- **历史记录**: 查看过往训练详情
- **数据统计**: 查看训练趋势和体重变化
- **运动库**: 管理和浏览运动动作

### PWA安装
- **Chrome**: 地址栏旁的"安装"按钮
- **Safari**: 分享菜单 → "添加到主屏幕"

## 📊 数据存储

- 所有数据存储在浏览器本地(IndexedDB)
- 支持数据导出和导入
- 无需注册账号，保护隐私
- 支持离线使用

## 🔧 开发说明

### 项目结构
```
src/
├── views/          # 页面组件
│   ├── Home.vue    # 首页
│   ├── Record.vue  # 记录页面
│   ├── History.vue # 历史记录
│   ├── Stats.vue   # 数据统计
│   ├── Settings.vue# 设置页面
│   └── ExerciseLibrary.vue # 运动库
├── stores/         # 状态管理
│   └── workout.ts  # 训练数据store
├── utils/          # 工具函数
│   └── database.ts # 数据库操作
├── router/         # 路由配置
├── styles/         # 全局样式
└── main.ts         # 应用入口
```

### 数据模型
- **WorkoutRecord**: 训练记录
- **Exercise**: 运动动作
- **ExerciseSet**: 训练组数据
- **UserSettings**: 用户设置

## 📄 许可证

MIT License

## 🤝 贡献

欢迎提交Issue和Pull Request！

## 📞 联系

如有问题或建议，请通过GitHub Issues联系。