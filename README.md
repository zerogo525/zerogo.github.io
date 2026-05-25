# 零启博客

基于 Hexo、Butterfly Theme 和 GitHub Pages 的个人博客系统。

## 技术栈

- Hexo 8
- Butterfly Theme
- GitHub Pages
- GitHub Actions

## 已配置能力

- 中文站点配置
- SEO 基础信息
- PrismJS 代码高亮
- 分类与标签页
- About 与 Projects 页面
- 深色模式
- 移动端样式优化
- 站点访问统计
- RSS: `/atom.xml`
- Sitemap: `/sitemap.xml`
- GitHub Pages 自动部署 workflow
- Hexo git 部署配置

## 本地开发

```bash
npm install
npm run server
```

## 生成静态文件

```bash
npm run build
```

## 部署

```bash
npm run deploy
```

当前 Hexo deploy 配置：

```yaml
deploy:
  type: git
  repo: https://github.com/zerogo525/zerogo.github.io.git
  branch: main
```

仓库地址：[zerogo525/zerogo.github.io](https://github.com/zerogo525/zerogo.github.io)

## GitHub Pages 设置

如果使用本仓库内的 GitHub Actions 自动部署，请在 GitHub 仓库中进入：

`Settings -> Pages -> Build and deployment -> Source -> GitHub Actions`

如果使用 `npm run deploy`，Hexo 会把生成后的 `public` 内容推送到 `main` 分支。
