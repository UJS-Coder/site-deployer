---
title: 真正的 Hello world
date: 2019-11-01 16:45:54
tags:
---

## Hello World, 这里是江苏大学计算机协会!

{% asset_img very-good.jpg very-good %}

### 我想写文章

本博客由 [hexo](https://hexo.io/zh-cn/ "hexo") 强力驱动，它是一个快速、简洁且高效的博客框架。文章可以使用 markdown 标记语言进行撰写。至于编辑器，我们可以自由选择，这篇文章是使用 [Editor.md](https://github.com/pandao/editor.md "Editor.md") 撰写的。

1 . 首先准备作业环境，你需要
git， 一台计算机

- 安装 git ，node.js
  前往 git 的[官网](https://git-scm.com/ "git")，nodejs 的[官网](https://nodejs.org/ "nodejs")，选择自己的系统对应的版本下载并且安装

- 克隆位于 github 上的 hexo 工作环境（Windows 在 powershell 中实现）

```bash
git clone https://github.com/UJS-Coder/site-deployer.git
cd site-deployer
```

- 安装 hexo

```bash
npm install hexo
```

至此，我们的工作环境已经部署完成！

2 . 撰写文章
我们可以先使用`hexo new [文章名]`创建一篇空白文章，执行完这条命令后，hexo 会在`source/_posts`目录下创建文件`[文章名].md`和空目录`/[文章名]`这样，我们就可以在`[文章名].md`里自由地撰写文章啦！
如果要在文章里摆放资源，我们可以把资源放到新创建的文件夹里，用

```
{% asset_img [图片名] [图片说明] %}
```

来代替资源。

3 .发布文章
使用`hexo g`命令来生成静态页面，我们可以再通过`hexo s`开启本地服务器在本地预览网页，确认~~完美~~后使用`hexo d`进行部署
此刻，我们的文章应该成功地发布在了社团的网页上，恭喜你！

### 注意事项

在撰文之前请务必确认本地的 hexo 工作目录时候和上游的状态一致，可以通过`git pull`与上游同步。若本地的 hexo 目录是过时的，在进行部署时可能会覆盖 github 上别人新发布的文章。
