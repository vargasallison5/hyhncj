VS平台主管【Q-——333307——】VS平台主管【 辋芷《888yx●vip》 】
VS平台主管【Q-——333307——】VS平台主管【 辋芷《888yx●vip》 】

 从零搭建个人博客：我用 GitHub Pages + Hexo 实现了自动化部署

作为一名前端开发者，我一直想拥有一个完全可控的个人技术博客。对比了 WordPress、掘金和知乎后，我最终选择了 GitHub Pages + Hexo 的组合方案。今天就把这套零成本、免服务器的建站流程分享出来，希望能帮你少踩几个坑。

 为什么选择 Hexo 而不是 VuePress？

很多朋友问我，现在 Vue 生态这么火，为什么不直接用 VuePress？我的核心考量有两点：

1. SEO 友好：Hexo 默认生成纯静态 HTML，百度爬虫收录效率极高。而 VuePress 的 SPA 架构在百度收录上会有一定延迟。
2. 主题生态丰富：Hexo 拥有超过 500 款成熟主题，尤其适合技术博客。我使用的 `NexT` 主题自带阅读进度条和文章目录，交互体验完全不输动态站。

 三步完成自动化部署

第一步：本地初始化
```bash
npm install hexo-cli -g
hexo init my-blog && cd my-blog
hexo g  生成静态文件
```

第二步：关联 GitHub 仓库
在 `_config.yml` 中修改 `deploy` 配置，只需要填入你的仓库地址即可。

第三步：开启 GitHub Actions
这是我重点推荐的功能。在仓库根目录创建 `.github/workflows/deploy.yml` 文件，写入自动化脚本后，每次你 `git push` 代码，GitHub 服务器就会自动构建并更新你的博客页面。完全摆脱了手动上传的烦恼。

 写给新手的三条优化建议

- 图片压缩：建议使用 `tinypng.com` 压缩图片，否则会拖慢首屏加载速度，影响用户体验。
- 内链建设：每篇文章至少关联 2 篇站内旧文，能有效降低跳出率，对百度 SEO 也非常有利。
- 主动提交收录：在百度搜索资源平台提交你的站点地图 `sitemap.xml`，最快 3 天就能被百度收录。

如果你在部署过程中遇到 `command not found` 报错，大概率是 Node 版本过低，升级到 16.x 以上即可解决。

你的第一个博客准备写点什么主题呢？ 欢迎在评论区和我聊聊你的建站计划，我会逐一回复。如果这篇文章对你有帮助，记得点个 在看 支持一下哦！

相关推荐：

https://github.com/gutierrezjessica05/nukelg/blob/main/2026%E6%9D%83%E5%A8%81%E7%83%AD%E6%A2%97%EF%BC%9AVS%E7%BD%91%E5%9D%80_%E6%80%9D%E8%87%80%E6%89%91%E5%85%91%E8%AE%ADSMGUN.md

<img src="https://i.postimg.cc/nzw2jbGZ/V8-00006.png" />

相关推荐：

https://github.com/gutierrezjessica05/nukelg/commit/cb0ba92bab216f423e365663775da614557e44f3

<img src="https://i.postimg.cc/2SFPqybC/V8-00015.png" />
相关推荐：

https://github.com/alexandersuzanne60/azaowe/blob/main/%E6%B7%B1%E5%BA%A6%E5%AE%9E%E6%93%8D%E6%95%99%E7%A8%8B%EF%BC%9AVS%E5%9C%B0%E5%9D%80_%E5%B4%AD%E8%B0%9D%E5%BD%A2%E7%84%B6%E5%83%AEFSSGA.md

<img src="https://i.postimg.cc/c4YqSXdK/V8-00012.png" />
相关推荐：

https://github.com/alexandersuzanne60/azaowe/commit/c4824e58d4baad011cf06692af2b8a86c5746481

<img src="https://i.postimg.cc/W4Nx0Vgy/V8-00017.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
