#### 电子书生成

+ 安装Gitbook
```
npm install  -g  gitbook-cli
```

+ 构建电子书
  + 这将把所有`.md`文件，转换成`.html`格式的静态文件，并存放在根目录下的`_book`目录
  + 要在自己的网站上发布新书，只需把_book目录复制到服务器相应目录即可。
```
gitbook build
```
+ 添加插件

  + Gitbook支持将一些外部的JavaScript文件嵌入到HTML中，例如Google统计、Disqus评论系统等。
  + 安装Disqus插件
```
npm install gitbook-plugin-disqus
```

在`book.json`中添加如下内容：

```
{
  "plugins": ["disqus"],
  "pluginsConfig": {
    "disqus": {
      "shortName": "你在Disqus上的项目名"
    }
  }
}
```