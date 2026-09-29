# display

内容归档站点（GitHub Pages 项目站）。

- 归档入口：https://chalersxu.github.io/display/
- 旅行攻略：https://chalersxu.github.io/display/travel/
- 家庭健康周报：https://chalersxu.github.io/display/fhi/

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

约 30 秒后生效。内容原件：旅行攻略在 `~/Documents/deepseek-harness/default-workspace/`，周报在 `~/Documents/DSH/FHI/reports/`；本仓库只存放发布副本。
