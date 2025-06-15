# Tauri + Vue 3

This template should help get you started developing with Tauri + Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

## Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) + [Tauri](https://marketplace.visualstudio.com/items?itemName=tauri-apps.tauri-vscode) + [rust-analyzer](https://marketplace.visualstudio.com/items?itemName=rust-lang.rust-analyzer)

## Tauri + Vue 3 桌面应用

这是一个使用 Tauri、Vue 3、Vite 和 Element Plus 构建的现代桌面应用程序。项目结构清晰，便于维护、修改和团队协作。

## 技术栈

- **Tauri**: 用于构建跨平台桌面应用
- **Vue 3**: 渐进式 JavaScript 框架
- **Vite**: 下一代前端构建工具
- **Element Plus**: Vue 3 UI 组件库

## 环境要求

在开始之前，请确保已安装以下软件：

- [Node.js](https://nodejs.org/) (v16 或更高版本)
- [Rust](https://www.rust-lang.org/tools/install)
- [Tauri CLI](https://tauri.app/v1/guides/getting-started/prerequisites)

## 项目设置

1. 克隆仓库：
```bash
git clone [仓库地址]
cd [项目名称]
```

2. 安装依赖：
```bash
npm install
```

## 开发模式

启动开发服务器：

```bash
npm run tauri dev
```

这将：
- 启动 Vite 开发服务器
- 在浏览器中打开 `http://localhost:5173/`
- 启动 Tauri 桌面应用窗口

## 生产构建

创建生产版本：

```bash
npm run tauri build
```

构建后的应用程序将位于 `src-tauri/target/release` 目录中。

## 项目结构

```
├── src/                    # Vue 源代码文件
│   ├── assets/            # 静态资源
│   ├── components/        # Vue 组件
│   ├── views/             # 页面组件
│   ├── router/            # Vue Router 配置
│   ├── store/             # Vuex 状态管理
│   ├── utils/             # 工具函数
│   ├── App.vue           # 根组件
│   └── main.js           # 应用入口文件
├── src-tauri/             # Tauri 后端
│   ├── src/              # Rust 源代码
│   └── tauri.conf.json   # Tauri 配置
├── public/                # 公共静态文件
├── index.html            # HTML 入口文件
├── vite.config.js        # Vite 配置
└── package.json          # 项目依赖和脚本
```

## 功能特点

- 使用 Element Plus 组件的现代化 UI
- 跨平台桌面应用
- 使用 Vite 实现快速开发
- 使用 Rust 实现类型安全的后端
- 响应式设计

## 开发规范

1. 代码风格
   - 使用 ESLint 进行代码检查
   - 遵循 Vue 3 官方风格指南
   - 组件名使用 PascalCase
   - 文件名使用 kebab-case

2. 目录结构
   - 组件按功能模块分类
   - 公共组件放在 components/common 目录
   - 业务组件放在 components/business 目录
   - 工具函数按功能分类放在 utils 目录

3. 命名规范
   - 变量使用 camelCase
   - 常量使用 UPPER_SNAKE_CASE
   - 组件名使用 PascalCase
   - CSS 类名使用 kebab-case

## 贡献指南

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/新功能`)
3. 提交更改 (`git commit -m '添加新功能'`)
4. 推送到分支 (`git push origin feature/新功能`)
5. 提交 Pull Request

## 许可证

本项目采用 MIT 许可证 - 详见 LICENSE 文件