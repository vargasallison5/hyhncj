VS主管【Q-——333307——】VS主管【 辋芷《888yx●vip》 】
VS主管【Q-——333307——】VS主管【 辋芷《888yx●vip》 】

 如何快速搭建个人博客？GitHub Pages + Hexo 完整教程

> 还在为买服务器、配数据库发愁？用 GitHub Pages 免费托管，30 分钟就能上线一个高速、稳定的个人博客。本文手把手教你从零开始，无需一行服务器代码，适合开发者、学生和写作爱好者。

 为什么选择 GitHub Pages 建博客？

- 完全免费：绑定自定义域名，不花一分钱
- 全球加速：依托 GitHub CDN，国内访问速度优秀
- 版本管理：文章 Markdown 格式，Git 历史记录可回溯
- 生态丰富：Hexo 主题超 500 款，插件一键安装

 第一步：环境准备（5 分钟）

你需要准备三个工具：
1. Node.js（建议 14+ 版本）
2. Git（Windows 用户安装 Git Bash）
3. GitHub 账号（免费注册）

安装完成后，打开终端输入 `node -v`，出现版本号即代表成功。

 第二步：快速搭建 Hexo 博客（10 分钟）

在终端输入以下命令，复制即可运行：

```bash
npm install hexo-cli -g
hexo init my-blog
cd my-blog
npm install
hexo server
```

打开浏览器访问 `http://localhost:4000`，看到默认页面就表示本地搭建成功。

 第三步：部署到 GitHub Pages（5 分钟）

1. 在 GitHub 新建仓库，命名为 `你的用户名.github.io`
2. 修改博客根目录的 `_config.yml` 文件：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

3. 安装部署插件并推送上线：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo generate && hexo deploy
```

访问 `https://你的用户名.github.io`，博客已正式上线！

 常见问题和优化技巧

- 图片加载慢？使用 GitHub 仓库存储图片，配合 CDN 加速
- SEO 优化？安装 `hexo-generator-seo-friendly-sitemap` 插件，自动生成站点地图
- 评论功能？集成 Gitalk 或 Valine，无需数据库

 行动起来吧！

建站只是第一步，持续输出才是关键。现在你可以：
1. 在 `source/_posts` 下新建 Markdown 文件写第一篇博文
2. 将博客链接分享到朋友圈、掘金、知乎，积累第一批读者
3. 收藏本文，遇到问题随时回查

> 互动提问：你准备用博客记录什么内容？技术笔记、生活感悟还是行业观察？欢迎在评论区留言，我会挑选典型需求出专题教程。

---

关键词：GitHub Pages 搭建博客、Hexo 教程、免费博客、个人网站搭建、静态网站托管

---

本文约 800 字，阅读时长 3 分钟。如果你觉得有帮助，欢迎点赞、收藏、转发，让更多朋友学会免费搭建高质量博客。

相关推荐：

https://github.com/gutierrezjessica05/nukelg/blob/main/%E5%A8%B1%E4%B9%90%E4%BA%A7%E4%B8%9A%E5%8A%A8%E6%80%81%EF%BC%9AVS%E5%9C%B0%E5%9D%80%E6%B3%A8%E5%86%8C_%E7%AB%BF%E5%B9%B8%E5%89%BF%E5%B4%A9%E8%B7%83SSZPX.md

<img src="https://i.postimg.cc/d0w4g90d/V8-00002.png" />

相关推荐：

https://github.com/gutierrezjessica05/nukelg/commit/d4ee051af22b377a8e2dfd5f5ceba35b3a9ec935

<img src="https://i.postimg.cc/YCfJ40GQ/V8-00016.png" />
相关推荐：

https://github.com/reidraymond02/imvanu/blob/main/2026%E5%AE%98%E7%BD%91%E6%94%BB%E7%95%A5%EF%BC%9AVS%E5%9C%B0%E5%9D%80%E5%BC%80%E6%88%B7_%E6%A1%88%E9%97%A8%E7%8A%B6%E6%81%8D%E9%80%9DDKEGN.md

<img src="https://i.postimg.cc/90Rpy8Ls/V8-00008.png" />
相关推荐：

https://github.com/reidraymond02/imvanu/commit/8e8bf3f86114750a4625aae52770f999e4cb6298

<img src="https://i.postimg.cc/SsKVxN8Z/V8-00004.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
