# display

内容归档站点（GitHub Pages 项目站）。

- 归档入口：https://chalersxu.github.io/display/
- 旅行攻略：https://chalersxu.github.io/display/travel/
- 家庭健康周报：https://chalersxu.github.io/display/fhi/

## 新增项目约定（2026-09-29 定，重要）

以后有新的发布内容，先分清是「新项目」还是「已有项目的新一期」：

| 情况 | 做法 | 得到的网址 |
|---|---|---|
| 已有项目出新内容（如又写了一期周报） | 在对应子目录里追加，入口页加/改一行 | 不变，如 `/display/fhi/2026-10-03/` |
| **全新项目** | **在本仓库根下新建 `display/<项目>/index.html`，并在根 `index.html` 的栏目列表里加一个入口** | `chalersxu.github.io/display/<项目>/` |

**约定：新项目一律是 display 仓库下的新子目录，不另开仓库。** 理由：链接风格统一（全部 `/display/...`）、只维护一套 Pages、不会出现多个仓库各自构建互相顶掉的情况。

原始内容（HTML/Markdown 原件）不放这里——本仓库只存发布副本。原件位置见下方「更新方式」。

## 目录结构

| 路径 | 用途 |
|---|---|
| `index.html` | 栏目导航（归档入口） |
| `travel/index.html` | 家庭旅行攻略（当前主推：昆明·抚仙湖·建水 2026 国庆） |
| `fhi/index.html` | 家庭健康周报归档页 |
| `fhi/<YYYY-MM-DD>/index.html` | 单期周报（日期＝统计窗口结束日） |

## 发布纪律

- 仓库为 public，Pages 内容公开可读；所有页面注入 `<meta name="robots" content="noindex,nofollow">`，不列入搜索引擎索引。
- 发布前扫描手机号 / 身份证 / 邮箱 / 具体门牌地址 / 家庭成员称呼。
- 周次 URL 固定为 `fhi/<窗口结束日>/`，与报告文件名对齐，链接永久稳定。

## 多份攻略演进

根下 `travel/index.html` 为当前主推攻略。新增第二份时，把当前这份移到 `travel/<trip-slug>/index.html`，`travel/index.html` 改为攻略导航页。

## 更新方式

```sh
git add -A && git commit -m "..." && git push
```

约 30 秒后生效。内容原件：旅行攻略在 `~/Documents/deepseek-harness/default-workspace/`，周报在 `~/Documents/DSH/FHI/reports/`。
