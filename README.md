# 澳新 17 天旅行手册

单文件、零外部依赖的旅行手册网页（`index.html`），手机打开快、离线可看。

## 部署（Cloudflare Pages · 免费 · push 即上线）

1. 本目录 push 到 GitHub 仓库（公开或私有均可）。
2. Cloudflare 控制台 → Workers & Pages → Create → Pages → Connect to Git，选这个仓库。
3. 框架预设选 **None**，构建命令留空，输出目录留空（根目录）。
4. Save and Deploy，完成后获得 `https://<项目名>.pages.dev` 公开网址。
5. 以后每次改完 `git push`，Cloudflare 自动重新发布。

> 说明：Cloudflare Pages 底层即 Workers 运行时，静态站点无需写 Worker 脚本。

## 本地预览

直接双击 `index.html` 用浏览器打开即可；或 `python3 -m http.server` 后访问 `http://localhost:8000`。
