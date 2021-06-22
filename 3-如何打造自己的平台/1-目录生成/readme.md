#### 目录生成

+ Summary简介：

[gitbook-summary](https://github.com/imfly/gitbook-summary)(简称Summary），它是一个自动构建文档目录的小工具。Summary默认将文件夹作为章节名称，文件夹嵌套对应目录结构。这样做，有很多好处，首先，把每一章的主题抽象为一个文件夹，然后把各章节独立成一个文件，放在该文件夹下，层次清晰，维护方便；其次，针对每一个概念，可以按照“面向对象”编程的思维去拆分，去写作。

+ 安装Summary

```
npm install -g gitbook-summary
```

+ 配置电子书信息

  + 进入项目根目录

  + 创建`book.json`
```
{
    "bookname": "My First Book",
    "description": "电子书生成测试",
    "author": {
        "name": "Tad",
        "email": "xiaozl1@digitalchina.com"
    },
    "keywords": [
        "gitbook",
        "summary"
    ]
}
```
+ 调整目录顺序

内容是有先后逻辑的。Summary默认按照章节（文件夹）的字母顺序排列。如果需要制定顺序，可以在文件夹前面加上字母或数字， 具体格式是:

```
{数字或字母}-文件夹或文件名称
```

比如：

```
1-Gitbook简介
```

+ 在每个叶子节点创建并编辑书籍正文

下图中可点击章节均为叶子节点，在其中创建`readme.md`即可被识别为章节内容
![2020-01-14-17-34-14](readme.assets/2020-01-14-17-34-14.png)

+ 生成目录文件`SUMMARY.md`

```
book sm
```
