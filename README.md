# 桌游工具箱

马里奥星星争夺战的轻量网页工具项目，使用 GitHub Pages 发布。

## 当前状态

已准备移动端适配的起始首页。骰子、计分板、计时器与规则查询仍待开发，首页明确显示各工具的状态。

## 技术结构

使用原生 HTML / CSS，后续交互使用 JavaScript。无安装依赖、无构建步骤。

- `index.html`：首页。
- `styles.css`：响应式样式。
- `.nojekyll`：让 GitHub Pages 直接发布静态文件。

该项目独立于 Python 对局引擎。第一版工具在浏览器内运行，计分计划保存在当前设备；多设备同步属于后续功能。

## 本地预览

在仓库目录运行：

```sh
python3 -m http.server 8080
```

打开 <http://localhost:8080>。

## 发布

在 GitHub 仓库的 **Settings → Pages** 中使用 **Deploy from a branch**，选择 `main` 分支和 `/ (root)`。启用后，推送到 `main` 会触发发布。

站点地址：<https://kio158.github.io/mario-game-tools/>

网页资源使用相对路径，兼容 GitHub Pages 的项目子目录。
