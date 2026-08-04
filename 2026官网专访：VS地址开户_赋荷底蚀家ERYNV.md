VS地址开户【Q-——333307——】VS地址开户【 辋芷《888yx●vip》 】
VS地址开户【Q-——333307——】VS地址开户【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025亲测有效）

大家好，我是老张。今天聊聊怎么用 GitHub Pages 免费搭建个人技术博客。如果你正在找一份最新、可操作的教程，这一篇应该能帮到你。全程不用买服务器，也不用懂后端，跟着做就行。

 为什么要用 GitHub Pages 搭博客？

首先，完全免费。无论是托管还是流量，都不花钱。其次，加载速度快，GitHub 的 CDN 在全球都有节点。更重要的是，Markdown 写作体验极佳，对程序员特别友好。你可以把博客当代码仓库管理，支持版本回滚，还能绑定自己的域名。

 第一步：准备环境（3分钟）

你需要准备三样东西：一个 GitHub 账号、安装好 Git 和 Node.js。Node.js 建议装 LTS 版本。检查好环境后，我们开始建仓库。

 第二步：创建仓库并开启 Pages

登录 GitHub，新建一个仓库，名字格式必须是：`用户名.github.io`。比如你的用户名是 `zhangsan`，仓库名就填 `zhangsan.github.io`。创建后，进入 Settings → Pages，把 Source 选为 `main` 分支，保存即可。

 第三步：本地安装 Hexo 框架（核心步骤）

在本地文件夹打开终端，执行以下命令：

```bash
npm install hexo-cli -g
hexo init blog
cd blog
npm install
hexo server
```

浏览器访问 `http://localhost:4000`，看到默认页面就说明成功了。这个框架支持主题切换，推荐使用 NexT 主题，在 `_config.yml` 里切换即可。写文章时，用 `hexo new post 文章标题` 创建文件，用 Markdown 语法编辑。

 第四步：一键部署上线（关键操作）

编辑根目录下的 `_config.yml`，找到 deploy 配置，改成你的仓库地址。然后安装部署插件：

```bash
npm install hexo-deployer-git --save
```

最后执行：

```bash
hexo clean && hexo generate && hexo deploy
```

等十几秒，访问你的 `用户名.github.io`，博客就上线了。

 常见问题排查建议

很多朋友卡在部署失败，通常是因为 SSH key 没配置好，或者仓库名写错。输入 `ssh -T git@github.com` 测试连接。如果提示 permission denied，重新生成密钥并添加到 GitHub 设置里。

看完这篇文章，你应该能顺利把博客跑起来了。如果你在搭建中遇到任何报错，请在评论区留言，我会在24小时内回复帮助解决。下一期准备写如何优化 SEO 和图片懒加载，感兴趣的话关注我，第一时间收到更新。

相关推荐：

https://github.com/gallowayhoward8/ohrtks/blob/main/2026%E6%9D%83%E5%A8%81%E6%B1%87%E6%80%BB%EF%BC%9AVS%E5%BC%80%E6%88%B7%E4%BB%A3%E7%90%86_%E8%B5%9D%E4%B9%88%E6%82%8D%E6%A1%A5%E5%B9%95GGFOV.md

<img src="https://i.postimg.cc/J7sVTRgT/V8-00010.png" />

相关推荐：

https://github.com/gallowayhoward8/ohrtks/commit/cdbe5aeb0588c556c50c170e0d5306c82f3c354c

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />
相关推荐：

https://github.com/fishergabrielle557/rvfthp/blob/main/2026%E6%9D%83%E5%A8%81%E4%B8%A5%E9%80%89%EF%BC%9AVS%E5%9C%B0%E5%9D%80%E5%A8%B1%E4%B9%90_%E5%85%86%E6%A1%88%E6%8D%A3%E8%B4%AA%E5%AD%A3HOVVP.md

<img src="https://i.postimg.cc/5tbnDmt0/V8-00001.png" />
相关推荐：

https://github.com/fishergabrielle557/rvfthp/commit/7e2b9a9e4705dc07401d8c2ea37eab60b3028577

<img src="https://i.postimg.cc/3Rw9xJm7/V8-00005.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
