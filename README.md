# web_test

## Cursor 学习页（单页面）

- 页面文件：`index.html`
- 在线预览地址（GitHub Pages）：<https://inernoro.github.io/web_test/>

## 已添加的 CI（自动部署到 GitHub Pages）

本仓库已添加工作流：`.github/workflows/pages.yml`

触发条件：

- 推送到 `main` 分支
- 手动触发（`workflow_dispatch`）

工作流会自动将仓库内容部署到 GitHub Pages。

## 如何配置（手把手）

1. 确认仓库中有 `index.html`（或你要发布的静态页面）。
2. 确认存在 `.github/workflows/pages.yml` 工作流文件。
3. 进入 GitHub 仓库页面：
   - `Settings` -> `Pages`
   - `Build and deployment` 选择 `Source: GitHub Actions`
4. 推送代码到 `main` 分支，等待 Actions 运行完成。
5. 首次部署成功后，访问：
   - `https://<你的GitHub用户名>.github.io/<仓库名>/`
   - 本仓库示例：<https://inernoro.github.io/web_test/>

## 你可以如何自定义

- 修改 `index.html` 内容后再次 push，页面会自动更新。
- 如果仓库名变化，访问地址也会变化：`/<新仓库名>/`。
- 如果是用户主页仓库 `<username>.github.io`，地址将是根域名（不带仓库路径）。

## UI/UX Pro Max Skill 安装与使用（Cursor）

已按你要求执行安装（当前仓库已生成 `.cursor/skills/ui-ux-pro-max`）：

```bash
npm install -g uipro-cli
uipro init --ai cursor
```

你本地也可以这样配置：

1. 安装 Node.js（建议 LTS）。
2. 执行上面两条命令。
3. 重启 Cursor。
4. 在对话里直接说：
   - `请帮我重做这个页面的 UI/UX`
   - `基于现代 SaaS 风格优化视觉层次和可读性`

更新技能版本：

```bash
uipro update
```