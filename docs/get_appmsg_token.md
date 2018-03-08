## 获取个人微信的相关参数

1. 打开fiddler开始监控
2. 登陆微信客户端，浏览该公众号的任意一篇推文
3. 可以观察到这里的内容显示会有阅读量、点赞量、评论等
4. 观察fiddler的监控数据，如下图显示

![fillder_1](https://raw.githubusercontent.com/wnma3mz/wechat_articles_spider/master/img/fillder_1.png)

5. 其中`/mp/getappmgsext?...`是我们推文内容的url，双击之后，fiddler界面右边出现如下图数据

![fillder_2](https://raw.githubusercontent.com/wnma3mz/wechat_articles_spider/master/img/fillder_2.png)

6.  从上图中的`WebForms`里面获取相关参数。上图下侧的json里面的`read_num`、`like_num`分别是阅读量和点赞量