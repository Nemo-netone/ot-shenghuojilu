# 旅行生活记录

## 在线演示

- Demo: https://ot-shenghuojilu.pages.dev
- GitHub: https://github.com/Nemo-netone/ot-shenghuojilu
- 管理员：`admin` / `admin`
- 普通用户：`用户账号1` / `123456`
- 运营人员：`运营01` / `123456`

## 原前端恢复

仓库保留原始项目源码，并在 `original-site/` 中提供可直接部署的恢复版前端。恢复方向为旅行记录与内容管理风格；`site/` 仅作为历史兜底，不再用于线上主页。

恢复版接入同源 Pages API，支持演示登录、游记列表，以及记录新增、编辑和删除。后端使用项目独立的 Supabase schema，不与其他作品集项目混用。

## 验证记录

2026-07-12 已完成稳定域名 HTTP 200、`/health`、全部公开演示账号登录、非空游记列表、临时记录新增/更新/删除与清理、桌面和移动端 Playwright 验证、浏览器控制台及失败资源检查。

![首页](docs/screenshots/home.png)
![管理页](docs/screenshots/admin.png)
![移动端](docs/screenshots/mobile.png)

## 本地预览

```bash
npx wrangler@3 pages dev original-site
```

## 许可

采用 PolyForm Noncommercial 1.0.0。允许非商业使用与修改；商业使用需另行获得作者许可。