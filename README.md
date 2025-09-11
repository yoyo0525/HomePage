# 🏠 阿布白（IonRh）的主页

## 🌐 在线演示
**演示站点：** http://home.loadke.tech/

> 使用原生 HTML、CSS、JS 构建，未依赖任何框架或插件，保证轻量高效。
> 增加，后台管理功能，更加方便新入坑的伙伴修改数据，不用直接修改源码

## ✨ 项目功能

- 🎨 **简洁美观** - 提供清爽的主页展示界面
- 📱 **响应式设计** - 完美适配手机、平板、桌面等各种设备
- ⚡ **极速加载** - 优化性能，提升用户浏览体验

## ⚙️ 使用说明

1. **部署后端**
1.上传 worker.js内容到cloudflare的Workers
如下图点击创建：
<img width="1767" height="969" alt="image" src="https://github.com/user-attachments/assets/15eb903e-e288-409e-8aca-2c7fca57fee1" />
点击如下图的开始使用：
<img width="1746" height="864" alt="image" src="https://github.com/user-attachments/assets/1590eea9-7f9c-42e4-855e-6aa6618aeb16" />
点击部署后，编辑代码：
<img width="2016" height="966" alt="image" src="https://github.com/user-attachments/assets/3b4ab43a-abac-4c24-8019-525c294a4cbc" />
将worker.js中的代码，复制到左侧的代码框，之后点击部署
<img width="2537" height="1311" alt="image" src="https://github.com/user-attachments/assets/3de35041-7db2-4297-a6c8-591f3cbdddaf" />
访问图中框住地方的域名，如：https://hoxxxx.xxxx.workers.dev/manage
即可看到后台管理界面
2.**后台界面**
   默认账号：`admin`，密码：`admin123`
<img width="936" height="635" alt="image" src="https://github.com/user-attachments/assets/23975bdb-cc30-47ee-87f7-9fb4bb07d333" />
后台管理界面：
<img width="1766" height="1227" alt="image" src="https://github.com/user-attachments/assets/f52ac415-88a6-476f-95e6-1f1099b92591" />

3. **home页部署方式**
部署好后，Fork 本仓库到你的 GitHub
修改仓库下的`/static/script.js`,`script.js`文件，修改如下图红框处的域名为,上面worker的域名（可自己修改worker域名）：`https://hoxxxx.xxxx.workers.dev`
<img width="2049" height="813" alt="image" src="https://github.com/user-attachments/assets/70c2778d-f84e-46c6-a830-61ee37423f3d" />
在 Cloudflare Pages 中新建站点并关联仓库，如下图：
<img width="2538" height="1092" alt="image" src="https://github.com/user-attachments/assets/1decf2ca-3864-4f9f-b308-ee9cdc7a5af3" />

4.就可以登陆管理界面，修改密码后，进行对应数据修改即可

## 📝 注意事项
- 如遇到问题，欢迎提交 Issue 反馈
- **修改时请保留原作者信息**

## 📸 页面预览
![主页截图](https://github.com/user-attachments/assets/de8bed1f-934e-4fee-958e-298becd5269f)
