# 部署说明

- Cloudflare Pages 项目：$repo
- 生产分支：main
- 发布目录：original-site/
- 稳定地址：https://ot-shenghuojilu.pages.dev
- API：同源 Pages Worker，入口位于 original-site/_worker.js
- 数据：项目隔离 Supabase schema，凭据仅配置在 Cloudflare secrets

2026-07-12 已真实部署并完成健康、登录、列表、CRUD、桌面和移动浏览器验证。site/ 为旧统一兜底页面，生产发布应使用 original-site/。