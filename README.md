# CCAIroom V3

状态：本轮首页与五个方法详情页已完成实现和三档响应式复测；2026-08-30 经 CC 审核通过并授权发布到 `www.ccairoom.cn`。

## 当前范围

- `index.html`：方法型首页。
- `methods/ai-story-factory.html`：AI 漫剧工厂详情页。
- `methods/ai-novel-factory.html`：AI 小说工厂详情页。
- `methods/ai-library.html`：AI 个人图书馆详情页。
- `methods/ai-visual-lab.html`：AI 影像实验室详情页。
- `methods/ai-project-management.html`：AI 多项目管理详情页。
- `assets/`：已通过的方法图、通用二维到三维示意与共享样式。

## 已验证

- 首页卡片、方法卡和图书馆／实验入口均可进入对应详情页。
- 1440、820、390 像素宽度下无页面横向溢出。
- 方法标题、流程节点标题与底部按钮无异常换行。
- 五个详情页图片均可正常加载。

## 本地预览

```bash
python3 -m http.server 41807 --bind 127.0.0.1
```

访问 `http://127.0.0.1:41807/`。

## 发布边界

- 本目录是已审核通过的 V3 发布源，不修改 `CCAIroom-V2`。
- 公开站展示个人 AI 方法与工作流，不包含公司素材、内部项目状态、本地路径、账号信息或私有运营数据。
- 正式发布保留既有 `CNAME`，并从远端 `main` 的隔离副本写入，避免带入历史工作区改动。
