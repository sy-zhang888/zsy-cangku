# HTML 页面骨架

生成新的概念学习资料时，复制下面的骨架，替换内容即可。保持单文件、无外部依赖。

## 骨架

```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>概念名 · 学习资料</title>
<style>
  :root{
    --ink:#2b2a27; --muted:#6b6862; --line:#e6e2d9;
    --paper:#fbfaf6; --card:#ffffff;
    --brand:#2f6f4f; --brand-soft:#eaf3ee;
    --accent:#b4652a; --accent-soft:#fbf0e6;
    --note:#3a5f8a; --note-soft:#eaf1f8;
  }
  *{box-sizing:border-box}
  body{
    margin:0; background:var(--paper); color:var(--ink);
    font-family:"PingFang SC","Hiragino Sans GB","Microsoft YaHei",sans-serif;
    font-size:16px; line-height:1.75;
  }
  .wrap{max-width:820px; margin:0 auto; padding:40px 22px 64px}
  h1{font-size:30px; margin:0 0 6px}
  .sub{color:var(--muted); margin-bottom:32px}
  section{
    background:var(--card); border:1px solid var(--line);
    border-radius:14px; padding:22px 24px; margin-bottom:20px;
  }
  h2{
    font-size:19px; margin:0 0 14px; padding-left:11px;
    border-left:4px solid var(--brand);
  }
  h3{font-size:16px; margin:18px 0 8px}
  table{width:100%; border-collapse:collapse; margin-top:10px; font-size:15px}
  th,td{border:1px solid var(--line); padding:9px 11px; text-align:left; vertical-align:top}
  th{background:var(--brand-soft); font-weight:600}
  .tag{
    display:inline-block; background:var(--accent-soft); color:var(--accent);
    border-radius:999px; padding:2px 11px; font-size:13px; margin-right:6px;
  }
  .warn{background:var(--note-soft); border-left:4px solid var(--note);
    border-radius:8px; padding:12px 15px; margin-top:12px}
  figure{margin:16px 0; text-align:center}
  figcaption{font-size:13px; color:var(--muted); margin-top:8px}
  details{border:1px solid var(--line); border-radius:9px; padding:10px 14px; margin-top:9px}
  summary{cursor:pointer; font-weight:600}
  ol.src{padding-left:22px; font-size:15px}
  ol.src li{margin-bottom:7px}
  a{color:var(--note)}
</style>
</head>
<body>
<div class="wrap">

  <h1>概念名</h1>
  <p class="sub">一句话定义，不超过 30 字</p>

  <section>
    <h2>学完你能做什么</h2>
    <ul>
      <li>目标一</li>
      <li>目标二</li>
      <li>目标三</li>
    </ul>
  </section>

  <!-- 其余板块按顺序：先问三个问题 / 它像什么 / 它怎么工作 / 用在哪儿 / 容易搞混 / 自测三题 / 资料来源 -->

</div>
</body>
</html>
```

## 配色说明

三种主色分别用于不同板块，避免全篇一个颜色：

- `--brand`（绿）：机制、流程类板块
- `--accent`（橙）：类比、案例类板块
- `--note`（蓝）：提示、边界、来源类板块

## 画图约定

- 用内联 `<svg>`，不用位图，不用外部图床
- `viewBox` 宽度统一 720，`width="100%"`，`height` 自适应
- 每个 svg 第一个子元素是 `<title>` 和 `<desc>`
- 图中每个关键部件都要有文字标注
- 只用纯色填充，不用渐变和阴影
