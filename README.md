在Git中，分支(branch)的概念非常重要，Git之所以强大，很大程度上就是因为它强大的分支体系。**这里的分支名字必须是gh-pages，因为github规定，只有该分支中的页面，才会生成网页文件**。
- _includes：默认的在模板中可以引用的文件的位置，后面会提到
- _layouts：默认的公共页面的位置，后面会提到
- _posts：博客文章默认的存放位置
- .gitignore：git将忽略这个文件中列出的匹配的文件或文件夹，不将这些纳入源码管理
- _config.yml：关于jekyll模板引擎的配置文件
- index.html：默认的主页

在_layouts目录下创建一个default.html，在其中输入如下内容，注意：文件本身要以UTF-8 without BOM的格式保存，以防止各种编码问题，建议使用notepad++或者VIM编辑
`<!DOCTYPE html>
<html>
<head>
　<meta http-equiv="content-type" content="text/html; charset=utf-8" />
　<title>一步步在GitHub上创建博客主页(2)</title>
</head>
<body>
　
</body>
</html>`

编辑index.html
`
---
layout: default
title: test title
---
<p>Hello world!</p>`

