# 旅行生活记录

![Demo Online](https://img.shields.io/badge/Demo-Online-brightgreen) ![Frontend](https://img.shields.io/badge/Frontend-Cloudflare%20Pages-f38020) ![License](https://img.shields.io/badge/License-Noncommercial-blue)

## 在线演示

- Demo: https://ot-shenghuojilu.pages.dev
- GitHub: https://github.com/Nemo-netone/ot-shenghuojilu
- 演示账号: $account

## 原前端恢复

本仓库保留原始项目源码，并在 original-site/ 中提供可直接部署的恢复版前端。恢复方向为：旅行记录与内容管理风格。统一 site/ 仅保留为历史兜底，不再作为线上主页面。

恢复版已接入同源 Pages API，支持演示登录、核心业务列表，以及记录新增、编辑和删除。后端继续使用项目独立 Supabase schema，不与其他作品集项目混用。

## 验证记录

2026-07-12 已完成：稳定域名 HTTP 200、/health、管理员登录、列表读取、临时记录新增/更新/删除并清理、桌面与移动端 Playwright 验证、浏览器控制台错误检查。

![首页](docs/screenshots/home.png)
![管理页](docs/screenshots/admin.png)
![移动端](docs/screenshots/mobile.png)

## 本地预览

`ash
npx wrangler@3 pages dev original-site
`

## 许可

采用 PolyForm Noncommercial 1.0.0。允许非商业使用与修改；商业使用需另行获得作者许可。