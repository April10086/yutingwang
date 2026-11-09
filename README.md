# 汪雨婷的个人学术主页

原生 HTML、CSS、JavaScript，无构建或后端依赖，资源均使用相对路径。沿用原模板布局、配色和响应式规则，包括移动端隐藏顶部导航的行为；仅对姓名增加了不换行及自适应字号修正。姓名：Yuting Wang / 汪雨婷；所在地：中国武汉；邮箱按本人提供的 wyt007@whut.eud.cn 保存。学院按“人工智能学院”处理。

## 本地预览

安装 Python 3 后，在 PowerShell 执行：

```powershell
cd 'D:\github个人界面'
python -m http.server 8000 --bind 127.0.0.1
```

浏览器打开 http://127.0.0.1:8000 。按 Ctrl+C 停止服务。也可直接打开 index.html。

## 修改个人内容

- `index.html`：姓名、身份、学院、地点、导师、联系方式、六个栏目和页脚。每个双语元素同时修改 `data-en`、`data-zh` 和标签内默认英文文本。
- `assets/site.js`：切换语言时的浏览器标题、网页描述、头像说明及导航标签。改姓名时也应同步此文件，以及 HTML 的 title、description、alt 和版权。
- `assets/styles.css`：原模板样式与姓名单行适配规则。
- `assets/portrait-placeholder.svg`：中性占位头像。照片放入 assets，并更新 HTML 的 img src 和 alt。
- 邮箱：修改侧栏邮件链接的 href 和显示文字，并同步页脚。当前为本人提供的 `wyt007@whut.eud.cn`。
- GitHub 已链接至 https://github.com/April10086 。ORCID 待补充；填写时添加真实 HTTPS 链接、`target="_blank" rel="me noreferrer"`，移除 aria-disabled，并更新双语文字。
- 简介和四项研究方向依据本人本地实验总结及周报概括；探索中的工作没有表述为已完成成果。教育经历已填写 2022–2026 本科、2026–至今硕士，均为武汉理工大学。论文、项目、荣誉暂为暂无，可沿用 CSS 中的 publication、project-card、honor 类补充真实内容。

待补充：ORCID（可不填）、照片（可不填）、论文/项目/荣誉（没有可保持暂无）。简介与研究方向可随研究进展更新。

## 部署 GitHub Pages

1. 在 GitHub 创建仓库，将本目录中的 index.html、assets、.nojekyll 和 README.md 放入仓库根目录。
2. 提交到 main 分支。
3. 仓库 Settings → Pages → Build and deployment → Source 选择 Deploy from a branch。
4. 选择 main 和 /(root)，保存，等待部署完成后打开 Pages 提供的网址。

可使用 `<用户名>.github.io` 仓库作为根站点，也可用普通项目仓库；相对资源路径兼容两者。

参考：[GitHub Pages 官方部署说明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。

