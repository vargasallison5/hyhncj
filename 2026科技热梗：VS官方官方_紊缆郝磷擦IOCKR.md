VS官方官方【Q-——333307——】VS官方官方【 辋芷《888yx●vip》 】
VS官方官方【Q-——333307——】VS官方官方【 辋芷《888yx●vip》 】

 从零搭建个人博客：用GitHub Pages免费部署静态网站

你是不是也想过拥有一个属于自己的博客？不用买服务器、不用备案，甚至不用花一分钱——GitHub Pages就能帮你实现。今天这篇教程，我会手把手带你完成从仓库创建到网站上线，整个过程大概只需要15分钟，适合零基础的新手。

 为什么选择GitHub Pages？

对于个人开发者、学生党或自由职业者来说，GitHub Pages有四个不可拒绝的优势：

1. 完全免费：托管在GitHub上，无限流量，无隐藏费用
2. 版本管理：每次更新都有记录，写错了可以随时回滚
3. 支持自定义域名：绑定自己的域名，看起来更专业
4. 无需服务器：静态网站部署简单，不需要配置后端环境

 第一步：创建你的第一个仓库

打开GitHub官网，登录后点击右上角的“+”号，选择“New repository”。

这里有个关键点：仓库名称必须设置为 `你的用户名.github.io`，比如如果你的用户名是 `zhangsan`，仓库名就是 `zhangsan.github.io`。这是GitHub Pages的固定规则，只有这个名称才能直接通过域名访问。

记得勾选“Public”（公开仓库），这样Pages服务才能正常工作。如果你想要私有仓库，需要开通付费版。

 第二步：选择你的建站方式

新手最推荐用 Jekyll主题，这是GitHub Pages原生支持的框架。你可以直接在仓库的Settings → Pages面板中，找到“Choose a theme”按钮，一键套用漂亮的模板。

如果你已经有现成的HTML/CSS文件，也可以直接上传到仓库根目录。我之前写过一篇《十分钟手写响应式个人主页》，感兴趣的朋友可以往前翻翻，里面详细讲了怎么用原生代码构建页面。

对于想玩得更花哨的朋友，推荐使用 Hugo 或 Hexo 这两个静态站点生成器。它们支持丰富的主题和插件，但需要本地安装环境，适合有一定命令行基础的读者。

 第三步：部署与发布

当你把代码推送到仓库后，GitHub会自动触发构建流程。你可以在仓库的 Actions 标签页里看到构建进度，一般30秒左右就能完成。

构建完成后，浏览器输入 `你的用户名.github.io` 就能看到你的网站了。每次更新代码，推送到主分支，页面会自动刷新，不需要任何手动操作。

 常见问题排查

Q：网站404了怎么办？  
A：检查仓库名称是否都是小写，确认主分支名称是 `main` 或 `master`，然后在Settings → Pages里确认Source选项选择了正确的分支。

Q：想绑定自己的域名怎么做？  
A：在仓库根目录创建一个名为 `CNAME` 的文件，文件内容填写你的域名。同时去你的域名DNS服务商那里添加一条CNAME记录，指向 `你的用户名.github.io`，等待解析生效即可。

 进阶玩法：动态内容不太适合

需要提醒的是，GitHub Pages只支持静态网页。如果你需要用户注册、评论功能、数据库交互这类动态操作，需要借助第三方服务，比如用 [GitHub Issues API](https://docs.github.com/en/rest/issues/issues?apiVersion=2022-11-28) 来搭建评论系统，或者用 [Cloudflare Workers](https://workers.cloudflare.com/) 做轻量的后端逻辑。

 行动起来吧

从创建仓库到网站上线，整个过程不需要安装任何软件，浏览器就能完成。如果你卡在哪一步，欢迎把报错信息发到评论区，我看到都会回复。

如果你成功用GitHub Pages搭好了博客，记得把链接贴在下面，让更多人看到你的作品。我会从中挑出三个有意思的博客，下期专门做一次好站推荐。

觉得有用的话，点个赞和在看，让更多想建站的朋友看到这篇教程。我们下篇文章见。

相关推荐：

https://github.com/fishergabrielle557/rvfthp/blob/main/%E8%B6%85%E5%85%A8%E5%AE%9E%E6%93%8D%E6%8C%87%E5%8D%97%EF%BC%9AVS%E5%9C%B0%E5%9D%80%E5%AE%A2%E6%9C%8D_%E7%AB%9E%E6%B0%90%E7%B3%96%E8%99%90%E5%85%88WJELZ.md

<img src="https://i.postimg.cc/J7sVTRgT/V8-00010.png" />

相关推荐：

https://github.com/fishergabrielle557/rvfthp/commit/335e88f3d96f3d45339f394600933d86785d4cf2

<img src="https://i.postimg.cc/5tbnDmt0/V8-00001.png" />
相关推荐：

https://github.com/gutierrezjessica05/nukelg/blob/main/2026%E7%AC%AC%E4%B8%80%E7%9B%98%E7%82%B9%EF%BC%9AVS%E5%9C%B0%E5%9D%80app_%E6%AD%89%E5%B9%B8%E5%90%AD%E7%A7%98%E6%93%9EOIVDE.md

<img src="https://i.postimg.cc/hGspn7JM/V8-00003.png" />
相关推荐：

https://github.com/gutierrezjessica05/nukelg/commit/6c18e8b56918702471a278cfd81a6a45d4380127

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
