# 瓢城花信 · 盐城双市花数字图鉴

一个纯静态单页网站，介绍江苏省盐城市的双市花——**牡丹（枯枝牡丹）**与**紫薇（百日红）**。

## 站点内容

| 路由 | 内容 |
| --- | --- |
| `#/home` | 首页 · 双花主视觉与城市速览 |
| `#/history` | 市花沿革时间轴（1991 → 2005） |
| `#/why` | 为什么盐城是双市花：自然 / 历史 / 社会三栏分析 |
| `#/peony` | 牡丹篇：便仓枯枝牡丹与文化意义 |
| `#/crape` | 紫薇篇：百日红与城市生活 |
| `#/route` | 两条赏花路线（春牡丹线 / 夏紫薇线） |
| `#/checkin` | 8 个赏花点打卡互动（localStorage 持久化） |

## 本地预览

直接双击 `index.html` 即可在浏览器打开。无需构建、无需后端。

## 部署到 GitHub Pages

### 方式一：网页端直接上传（最快）

1. 在 GitHub 新建一个仓库，名字建议 `yancheng-flowers`（公开仓库）。
2. 进入仓库主页，点击 **Add file → Upload files**。
3. 把整个 `yancheng-flowers` 文件夹里的**所有文件**（`index.html`、`README.md`、`assets/` 整个目录）拖进去。
4. 点击底部 **Commit changes**。
5. 进入仓库 **Settings → Pages**：
   - **Source** 选 `Deploy from a branch`
   - **Branch** 选 `main`，文件夹选 `/ (root)`
   - 点 **Save**
6. 等待 1–2 分钟，GitHub 会给出访问地址：
   `https://<你的用户名>.github.io/yancheng-flowers/`

### 方式二：命令行推送

```bash
cd yancheng-flowers
git init
git add .
git commit -m "init: yancheng dual city flowers guide"
git branch -M main
git remote add origin https://github.com/<你的用户名>/<仓库名>.git
git push -u origin main
```

然后同样去 **Settings → Pages** 开启即可。

## 目录结构

```
yancheng-flowers/
├── index.html          # 单文件应用，含全部样式与脚本
├── README.md
└── assets/
    ├── hero.jpg        # 首页工笔主视觉
    ├── peony.jpg       # 牡丹特写
    ├── crape.jpg       # 紫薇街景
    └── garden.jpg      # 便仓枯枝牡丹园
```

## 数据来源

- 盐城市史志网《盐城地情》
- 盐城市档案馆《盐城大事记 2005.7》
- 盐城新闻网《市区紫薇盛放期》(2025-08)
- 《盐城年鉴 2025》
- 中国江苏网、国际在线江苏频道相关报道
