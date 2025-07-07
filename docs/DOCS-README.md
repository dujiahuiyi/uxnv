# Hajimi 文档站点

这是 Hajimi 项目的 VuePress 文档站点，提供完整的使用指南和部署教程。

## 🚀 快速开始

### 本地开发

```bash
# 安装依赖
cd docs
npm install

# 启动开发服务器
npm run docs:dev

# 访问 http://localhost:8080
```

### 构建生产版本

```bash
# 构建静态文件
npm run docs:build

# 生成的文件在 .vuepress/dist 目录
```

## 📁 目录结构

```
docs/
├── .vuepress/
│   ├── config.js          # VuePress 配置
│   ├── public/            # 静态资源
│   └── styles/            # 自定义样式
├── deploy/                # 部署指南
│   ├── README.md          # 快速开始
│   ├── docker.md          # Docker 部署
│   ├── huggingface.md     # Hugging Face 部署
│   ├── claw.md            # Claw Cloud 部署
│   ├── zeabur.md          # Zeabur 部署
│   ├── termux.md          # Termux 部署
│   └── vertex.md          # Vertex AI 配置
├── usage/                 # 使用指南
│   ├── README.md          # 基本使用
│   ├── configuration.md   # 配置说明
│   └── troubleshooting.md # 故障排除
└── README.md              # 首页
```

## 🎨 自定义

### 修改主题颜色

编辑 `.vuepress/styles/index.styl`：

```stylus
// 主色调
$accentColor = #667eea
$textColor = #2c3e50
$borderColor = #eaecef
```

### 添加新页面

1. 在相应目录下创建 `.md` 文件
2. 在 `.vuepress/config.js` 中更新侧边栏配置

### 自定义组件

在 `.vuepress/components/` 目录下创建 Vue 组件。

## 🚀 部署

### GitHub Pages

项目已配置自动部署，推送到 `doc` 分支后会自动构建并部署到 GitHub Pages。

访问地址：`https://username.github.io/hajimi/`

**部署步骤**：
1. 将文档更改推送到 `doc` 分支
2. GitHub Actions 自动触发构建
3. 构建完成后自动部署到 GitHub Pages

### 其他平台

生产构建后，将 `.vuepress/dist` 目录的内容部署到任何静态网站托管服务。

## 📝 内容更新

### 添加新的部署方式

1. 在 `deploy/` 目录创建新的 `.md` 文件
2. 更新 `deploy/README.md` 的部署方式列表
3. 在 `.vuepress/config.js` 中添加到侧边栏

### 更新配置说明

编辑 `usage/configuration.md` 文件，按照现有格式添加新的配置项。

### 添加故障排除

在 `usage/troubleshooting.md` 中添加新的常见问题和解决方案。

## 🔍 搜索优化

文档已配置 SEO 优化：

- 语义化的页面标题
- 完整的 meta 描述
- 结构化的内容层级
- 友好的 URL 结构

## 📞 维护

### 定期更新

- 检查外部链接的有效性
- 更新软件版本号
- 同步最新的功能特性
- 优化用户反馈的内容

### 监控

使用 GitHub Issues 跟踪文档相关的问题和改进建议。

---

如有问题或建议，请在 [GitHub Issues](https://github.com/wyeeeee/hajimi/issues) 中反馈。