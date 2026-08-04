VS平台主管【Q-——333307——】VS平台主管【 辋芷《888yx●vip》 】
VS平台主管【Q-——333307——】VS平台主管【 辋芷《888yx●vip》 】

 如何用 GitHub Actions 自动部署博客？看完这篇你就会了

作为一名开发者，你是不是也遇到过这样的烦恼：每次写完博客，都要手动执行构建、上传服务器，既费时又容易出错。今天就教大家用 GitHub Actions 实现自动化部署，让你专注写作，其他交给脚本。

 什么是 GitHub Actions？

简单来说，GitHub Actions 是 GitHub 自带的 CI/CD 工具，你可以在仓库里定义工作流，当代码推送、PR 合并时自动触发构建和部署任务。免费、无需额外服务器，是个人博客自动化的首选方案。

 三步搞定自动化部署

 第一步：准备部署密钥
在仓库 Settings -> Secrets 中添加部署服务器的 SSH 私钥（或云厂商 Access Key），记住变量名，比如 `DEPLOY_KEY`。这是安全考量，避免在代码中暴露敏感信息。

 第二步：编写工作流文件
在项目根目录创建 `.github/workflows/deploy.yml`，核心配置如下：

```yaml
name: Auto Deploy
on:
  push:
    branches: [ main ]
jobs:
  build-and-deploy:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3
      - uses: actions/setup-node@v3
        with:
          node-version: 18
      - run: npm ci && npm run build
      - name: Deploy to Server
        uses: easingthemes/ssh-deploy@v2
        with:
          SSH_PRIVATE_KEY: ${{ secrets.DEPLOY_KEY }}
          SOURCE: "dist/"
          TARGET: "/var/www/blog"
```

 第三步：推送触发自动部署
把代码推送到 main 分支，Actions 就会自动运行。在仓库的 Actions 选项卡里，你可以实时查看部署日志，失败了会红点提示，方便排查。

 常见问题与解决

- 构建超时：把 `timeout-minutes` 加到 job 级别，默认是 6 小时，一般够用。
- 密钥无效：检查是否多复制了换行符，格式错误是头号杀手。
- 中文路径乱码：在部署前加 `- run: chmod +x deploy.sh` 并设置 UTF-8 编码。

 总结与互动

GitHub Actions 不止能部署博客，还能自动化测试、自动发布 Release、定时爬虫任务。学会这个技能，你的开发效率会提升一个档次。

你在用 GitHub Actions 做什么？遇到过什么坑？欢迎在评论区分享你的经验，或直接点赞收藏方便以后查。 关注我，每天分享开发工具小技巧，让技术生活更简单。

相关推荐：

https://github.com/vargasallison5/hyhncj/blob/main/2026%E7%AC%AC%E4%B8%80%E4%B8%93%E8%AE%BF%EF%BC%9AVS%E4%B8%8B%E8%BD%BD_%E7%BD%AE%E6%B1%95%E5%BB%96%E7%8E%B0%E5%A0%86EERDQ.md

<img src="https://i.postimg.cc/90Rpy8Ls/V8-00008.png" />

相关推荐：

https://github.com/vargasallison5/hyhncj/commit/04eee43f41f53b45f4a380bad00cbb3b90b06318

<img src="https://i.postimg.cc/SKg3rPf5/V8-00018.png" />
相关推荐：

https://github.com/gallowayhoward8/ohrtks/blob/main/%E6%BC%AB%E6%B8%B8%E6%96%87%E5%A2%83%E8%BF%BD%E6%A2%A6%EF%BC%9AVS%E5%AE%A2%E6%9C%8D_%E5%93%81%E7%96%B5%E7%BF%B0%E5%8D%97%E6%BB%A5XXSKY.md

<img src="https://i.postimg.cc/tJZ5FSB6/V8-00007.png" />
相关推荐：

https://github.com/gallowayhoward8/ohrtks/commit/92bd9affaa1bd07c3724996aa10f7804c43c770d

<img src="https://i.postimg.cc/d05pBf9J/V8-00019.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
