# Static Site Starter

一个无依赖、可快速改文案并上线的静态网站骨架。当前视觉方向是深色 editorial / studio 风格，适合产品落地页、个人作品集、轻量官网、活动页。

## Files

- `index.html`：页面结构与文案内容
- `styles.css`：完整视觉样式、响应式布局、动效
- `script.js`：滚动进入视口的 reveal 动画
- `dist/`：`npm run build` 生成的静态部署产物

## Commands

```bash
npm run dev
npm run build
npm run preview
```

默认本地预览端口是 `4173`。

## Edit Checklist

1. 替换 `index.html` 中的品牌名、标题、副标题、服务项和联系方式。
2. 如果要换主题色，优先修改 `styles.css` 顶部 `:root` 里的 CSS 变量。
3. 执行 `npm run build`，确认 `dist/` 里生成 `index.html`、`styles.css`、`script.js`。
4. 将 `dist/` 部署到 Vercel、Netlify、Cloudflare Pages、GitHub Pages 或任意静态托管。

## Deploy

### Vercel

- Framework Preset: `Other`
- Build Command: `npm run build`
- Output Directory: `dist`

### Netlify

- Build Command: `npm run build`
- Publish Directory: `dist`

### GitHub Pages

当前仓库发布到 `gh-pages` 分支，GitHub Pages Source 使用 `Deploy from a branch`，分支选择 `gh-pages` / root。

手动发布流程：

1. 执行 `npm run build` 生成 `dist/`。
2. 将 `dist/` 内容发布到 `gh-pages` 分支根目录。
3. 在 GitHub Pages 构建完成后访问 `https://cxb-soft.github.io/orie.dev/` 验证。

```bash
npm run build
```

## Status

- Build verified with `npm run build`.
- Initial Git commit: `0963c42 feat: create distinctive static landing page starter`.
