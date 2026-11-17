# my-first-site

我的第一个网址。做它的目的不是好看，是证明我能把东西从零做到上线。

## 这是什么

天津理工大学中环信息学院软件工程大一学生的个人主页，也是 8 周计划里第 1 周的交付物。

## 怎么打开

- 本地：双击 `index.html`
- 线上：推到 GitHub 并开启 Pages 后，访问 `https://y-q-bobo.github.io/my-first-site/`

## 目录

```
my-first-site/
├── index.html                  页面结构
├── css/style.css               样式 + 手机适配
├── img/                        图片（暂时为空）
├── .github/workflows/deploy.yml 自动部署到 GitHub Pages
├── .gitignore
└── README.md
```

## 已完成的 8 周目标

- [x] 第 1 周：跑通「改代码 → 提交 → 上线」
- [x] 第 2 周：375px 宽度下不换行（已实测 `scrollWidth=375`）
- [ ] 第 4 周：做出成绩工具的静态版
- [ ] 第 8 周：完整交付（网址 + README + 视频）

## Git 提交记录

```
a86204a 细节：补正文首句后的全角空格，避免标点粘连
5f004d1 加自动部署：push 到 main 后由 GitHub Actions 发布到 Pages
b07c98b 手机适配：375px 宽度下不换行、按钮竖排
aa5c7d6 加样式：深蓝配色、卡片布局、头像和按钮
c576b23 建站：写下主页结构和自我介绍
```

## 怎么推到 GitHub（还需要你做一步）

现在 `origin` 指向的是本地演示仓库 `E:\Projects\remote-demo.git`，用来先把 push 跑通。
换成你自己的 GitHub 仓库，执行下面三行（把 `你的用户名` 换掉）：

```bash
cd /e/Projects/my-first-site
git remote set-url origin https://github.com/y-q-bobo/my-first-site.git
git push -u origin main
```

然后到 GitHub 仓库页：**Settings → Pages → Source 选 GitHub Actions**，等 1 分钟，网址就有了。

第一次 push 会要求登录。弹窗里选 **Sign in with your browser**，用浏览器授权一次即可，之后不用再输。

## 每天的日常（三条命令）

```bash
git add .
git commit -m "一句话说明今天改了什么"
git push
```

## 更新记录

- 2026-11-17：建站、加样式、手机适配、配置自动部署，共 5 次提交

## 已经替你配好的部分

- 远程 `origin` 已指向 `https://github.com/y-q-bobo/my-first-site.git`
- 桌面/项目内的 `推送到GitHub.bat` 可一键推送（会弹浏览器授权）
- `检查状态.bat` 可随时检查远程地址、提交历史和仓库是否已建

## 你还需要做的两步

1. 在 GitHub 建空仓库 `my-first-site`（不要勾 Add README）
2. 双击 `推送到GitHub.bat`，浏览器弹出时点授权

## 为什么这一步不能代做

推送需要 GitHub 授权。机器的凭据助手是 `helper-selector`（Git Credential Manager），
授权动作必须由账号本人在浏览器里确认；把 token 交给我也不建议，那等于交出账号写权限。