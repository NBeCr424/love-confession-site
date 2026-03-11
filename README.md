# 暖暖猫咪幸运站

一个可直接部署到 GitHub Pages 的静态互动站点，包含三层流程：

1. 第一层：填写并保存用户信息（localStorage）
2. 第二层：抽取今日幸运签（含历史记录）
3. 第三层：名字小诗 + 猫咪换装 + 纪念海报导出

## 本地预览

1. 直接打开 `index.html`
2. 或运行：
   - `./serve.ps1`
   - 浏览器访问 `http://localhost:5500/`

## 发布到 GitHub Pages

### 一键脚本

1. 先登录 GitHub CLI：`gh auth login`
2. 执行：`./publish-gh-pages.ps1 -RepoName warm-cat-lucky-site -Visibility public`

### 手动方式

1. `git add .`
2. `git commit -m "update warm cat site"`
3. `git push origin main`
4. 在 GitHub 仓库 Settings -> Pages 中选择：
   - Source: Deploy from a branch
   - Branch: `main` / `(root)`

部署完成后公网地址通常为：
`https://<github-username>.github.io/<repo-name>/`
