# 功能说明

## 项目定位

围绕城市、景点、旅行记录、攻略、行程规划和论坛的生活记录演示系统。

## 功能树

| 模块 | 责任 | 数据归属 |
|---|---|---|
| 城市管理 | 城市、区域、标签和推荐信息 | `items.module_key = city` |
| 景点信息 | 景点类型、门票、开放时间和详情 | `items.module_key = scenic` |
| 旅行记录 | 用户游记、图片、时间和路线 | `items.module_key = record` |
| 旅游攻略 | 攻略、收藏、评论和推荐 | `items.module_key = guide` |
| 行程规划 | 行程安排、日期、城市和状态 | `items.module_key = plan` |
| 旅行论坛 | 帖子、举报、敏感词和互动 | `items.module_key = forum` |

## 使用场景

1. 访客打开 `https://ot-shenghuojilu.pages.dev`，先浏览项目定位、核心模块和演示账号。
2. 使用公开账号登录，进入工作台查看统计数据。
3. 通过模块侧边栏进入业务表，进行列表浏览、关键词搜索、新增、编辑和删除。
4. 管理员可完整演示数据维护流程；普通用户和工作人员账号用于展示不同角色入口。

## 调用链和数据流

```text
浏览器
  -> site/app.js
  -> /api/login 或 /api/items/*
  -> site/_worker.js
  -> Supabase RPC public.ot_shenghuojilu_demo_rest
  -> ot_shenghuojilu.accounts / ot_shenghuojilu.items
```

## 推荐演示路径

```text
登录 -> 工作台统计 -> 城市管理 -> 景点信息 -> 旅行记录 -> 旅游攻略 -> 新增一条记录 -> 编辑状态 -> 删除测试记录
```

## 演示边界

- 已实现：登录、统计、业务模块列表、搜索、新增、编辑、删除。
- 部分实现：原项目的复杂权限、文件上传、第三方服务以作品集展示为主。
- 未接入：真实支付、短信、地图、邮件、生产级文件存储。
