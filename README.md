# 🏠 阿布白（IonRh）的主页

一个使用原生 HTML、CSS、JS 构建的个人主页项目，未依赖任何框架或插件，保证轻量高效。包含前端展示页面和后台管理系统，让你轻松定制自己的个人主页。

## 🌐 在线演示

**演示站点：** http://home.loadke.tech/

## ✨ 项目特色

- 🎨 **简洁美观** - 提供清爽的主页展示界面
- 🌐 **后台管理** - 提供方便的后台数据管理系统
- 📱 **响应式设计** - 完美适配手机、平板、桌面等各种设备
- ⚡ **极速加载** - 原生代码构建，优化性能，提升用户浏览体验
- 🔧 **易于定制** - 通过后台管理界面轻松修改数据，无需直接修改源码

## 🚀 快速开始

### 第一步：部署后端服务（Cloudflare Workers）

1. **创建 Worker**
   - 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)
   - 进入 Workers & Pages 页面
   - 点击 "创建应用程序" → "创建 Worker"

   <img width="1767" height="969" alt="创建Worker" src="https://github.com/user-attachments/assets/15eb903e-e288-409e-8aca-2c7fca57fee1" />

2. **配置 Worker**
   - 点击 "开始使用"

   <img width="1746" height="864" alt="开始使用" src="https://github.com/user-attachments/assets/1590eea9-7f9c-42e4-855e-6aa6618aeb16" />

3. **部署代码**
   - 点击 "部署" 后，选择 "编辑代码"

   <img width="2016" height="966" alt="编辑代码" src="https://github.com/user-attachments/assets/3b4ab43a-abac-4c24-8019-525c294a4cbc" />

   - 将 `worker.js` 文件中的代码完整复制到左侧代码编辑器中
   - 点击 "部署" 完成部署

   <img width="2537" height="1311" alt="部署代码" src="https://github.com/user-attachments/assets/3de35041-7db2-4297-a6c8-591f3cbdddaf" />

4. **获取访问地址**
   - 部署成功后，记录下你的 Worker 域名，格式如：`https://your-worker-name.your-subdomain.workers.dev`

### 第二步：配置后台管理

1. **访问后台管理界面**
   - 在浏览器中访问：`https://your-worker-domain/manage`
   - 默认登录信息：
     - 用户名：`admin`
     - 密码：`admin123`

   <img width="936" height="635" alt="登录界面" src="https://github.com/user-attachments/assets/23975bdb-cc30-47ee-87f7-9fb4bb07d333" />

2. **后台管理功能**
   - 登录后即可看到管理界面，可以管理个人信息、项目展示等数据

   <img width="1766" height="1227" alt="管理界面" src="https://github.com/user-attachments/assets/f52ac415-88a6-476f-95e6-1f1099b92591" />

### 第三步：部署前端页面（Cloudflare Pages）

1. **Fork 项目**
   - Fork 本仓库到你的 GitHub 账户

2. **修改配置文件**
   - 编辑 `/static/script.js` 文件
   - 将文件中的 API 域名修改为你在第一步中获得的 Worker 域名：
     ```javascript
     const API_BASE = 'https://your-worker-domain.workers.dev';
     ```

   <img width="2049" height="813" alt="修改配置" src="https://github.com/user-attachments/assets/70c2778d-f84e-46c6-a830-61ee37423f3d" />

3. **部署到 Cloudflare Pages**
   - 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)
   - 进入 Workers & Pages 页面
   - 点击 "创建应用程序" → "Pages" → "连接到 Git"
   - 选择你 Fork 的仓库并完成部署配置

   <img width="2538" height="1092" alt="部署Pages" src="https://github.com/user-attachments/assets/1decf2ca-3864-4f9f-b308-ee9cdc7a5af3" />

### 第四步：完成配置

1. **修改默认密码**
   - 首次登录后台管理界面后，请立即修改默认密码
   - 在管理界面中更新你的个人信息、项目展示等数据

2. **测试访问**
   - 访问你的 Pages 域名，查看个人主页效果
   - 确认后台管理功能正常工作

## 📋 项目结构

```
HomePage/
├── static/           # 前端静态文件
│   ├── index.html   # 主页面
│   ├── script.js    # 主要脚本（需要修改API地址）
│   └── style.css    # 样式文件
├── worker.js        # Cloudflare Worker 后端代码
└── README.md        # 项目说明文档
```

## 🔧 自定义配置

- **修改样式**：编辑 `static/style.css` 文件
- **修改内容**：通过后台管理界面更新数据
- **修改功能**：编辑 `static/script.js` 和 `worker.js` 文件

## 📝 注意事项

- ⚠️ 请务必修改默认的管理员密码
- 🔗 确保 Worker 域名配置正确，否则前端无法正常获取数据
- 🌐 如需自定义域名，请在 Cloudflare 中进行相应配置
- 📱 项目已适配移动端，无需额外配置
- 🐛 如遇到问题，欢迎提交 Issue 反馈

## 📄 许可证

**修改时请保留原作者信息**

## 📸 页面预览

![主页截图](https://github.com/user-attachments/assets/de8bed1f-934e-4fee-958e-298becd5269f)
