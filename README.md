# 虎跃使用指南 - 静态站点

可直接部署的纯静态 HTML/CSS/JS 网站。

## 主要目录

- `/huyue/`：虎跃安装、使用和设备故障指南
- `/chatgpt/`：ChatGPT 网络、登录与验证问题
- `/youtube/`：YouTube 播放、电视端与内容不可用问题
- `/netflix/`：Netflix 地区、VPN / Proxy 与影片不可用问题
- `/telegram/`：Telegram 连接、验证码与代理问题
- `/disney-plus/`：Disney+ 地区、播放与 Error 43 / 93 问题
- `/tiktok/`、`/x/`：对应平台的网络与地区问题
- `/network/`：通用网络和 DNS 排查

## 上传前修改站点地址

全站已配置为 GitHub Pages 组织站根地址：

- 用户/组织 Pages：`https://yourname.github.io`
- 独立域名：`https://example.com`

根地址末尾不要额外添加 `/`。替换范围包括 canonical、Open Graph、JSON-LD、`sitemap.xml`、`robots.txt` 和 `llms.txt`。

## GitHub Pages

当前内部链接使用根路径形式，例如 `/huyue/how-to-use/`，适合用户/组织 Pages 或独立域名。若部署到 `username.github.io/repository/` 这种项目子路径，需要统一加入仓库前缀。

上传时保留 `.nojekyll`。当前文件默认按 `username.github.io` 根站点设计；如果使用项目子路径，请先统一调整根路径。部署后检查首页、404、移动端导航、图片和主要文章是否能正常打开。

## 图片

`assets/images/huyue-app-home.webp` 为社交分享和高密度屏幕使用的虎跃客户端真实截图；`huyue-app-home-384.webp` 为较小屏幕准备的响应式版本。成品包不再附带未压缩 PNG，减少仓库和部署体积。
