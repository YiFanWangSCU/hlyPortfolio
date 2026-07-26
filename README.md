# 作品集静态站点

部署时，把这个目录的所有文件作为 Cloudflare Pages 或 GitHub Pages 的发布根目录。

## 后续更新作品集

只需要把新的 PDF 替换为同目录下、同名的 `portfolio.pdf`。不要改动 `index.html`。

网页会自动整页展示该 PDF；如果访客的浏览器不支持内嵌预览，也可以在新标签页打开 PDF。

## Cloudflare Pages（推荐）

1. 将本目录的文件上传到一个 GitHub 仓库的根目录。
2. 在 Cloudflare Dashboard 的 **Workers & Pages** 中创建 Pages 项目并连接该 GitHub 仓库。
3. Framework preset 选 **None**；Build command 留空；Build output directory 填 `.`。
4. 部署后，在项目的 **Custom domains** 中绑定 `portfolio.0121f.online`。

Cloudflare 会自动配置 HTTPS。若域名 DNS 不在 Cloudflare，请按其提示添加 CNAME 记录；若已托管在 Cloudflare，通常可直接由页面自动创建记录。
