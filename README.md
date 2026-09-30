# 和光 AI 空间 · 共居共建伙伴招募页

> 和其光，同其尘。——《道德经》

和光 AI 空间（杭州·首章新所）的伙伴招募落地页。

## 线上地址

| 线路 | 地址 |
| --- | --- |
| GitHub Pages | https://ashes-fish.github.io/heguang-space/ |
| 国内镜像 | https://heguang-space-80645.app.workbuddy.host/ |

## 这是什么

**零外链单文件页面。** 全部 CSS、JavaScript、26 张照片（base64 内联）都装在 `index.html` 这一个文件里，约 1.5 MB。页面不发出任何外部请求，双击本地打开即可运行，也可以丢进任意静态托管。

## 仓库里有什么

```
index.html    发布产物本体（唯一的页面文件）
.nojekyll     关掉 Jekyll 处理，让文件原样发布
README.md     本文件
```

## 这不是源文件

本仓库只存放**发布产物**，是面向上线的快照，不是日常编辑的地方。

真正在维护的源文件在项目工作区：

```
<工作区>/heguang-space/index.html
```

页面结构（9 段叙事 + 5 个详情弹层）、动效参数、图片处理流程等约束都记录在工作区的项目记忆中。

## 更新流程

```bash
# 1. 在源文件处改好、验证好
# 2. 复制产物到本目录
cp heguang-space/index.html _deploy/github/index.html

# 3. 提交推送
cd _deploy/github
git add -A
git commit -m "更新：<改了什么>"
git push
```

推送后 GitHub Pages 会在 1～2 分钟内自动重新构建。

**注意**：必须覆盖本目录的 `index.html`，不要另存成别的文件名——Pages 只认根目录的 `index.html`。

## 页面构成

九个区块，一次滚动读完：

序章 → 主张 → 现场 → 聚光 → 入圈

| 区块 | 内容 |
| --- | --- |
| Hero | 和其光 / 同其尘 |
| 主张段 | 逐字点亮的长句 |
| 数据 | 单间 900 元/月起、算力激励、AI 夜校、在册成员 |
| 五卡 | 和光公寓 / 夜光计划 / 流光网络 / 生活现场 / 社区共识 |
| 聚光 | 粒子汇聚动效 |
| 入圈 | 联系方式（占位） |

五张卡片可点击，各自弹出详情层。

## 待办

- [ ] 页脚联系方式仍是占位，需替换成真实微信 / 邮箱
- [ ] 补上 OG 标签（`og:title` / `og:image` / `og:description`），否则分享到微信、小红书只有裸链接没有缩略图
- [ ] `<meta name="description">` 仍是旧文案，待与全站定位统一
- [ ] 封面图 C2 / C3 / C5 仍是占位
