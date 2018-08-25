# 项目初始化步骤

## 1、安装基础环境
- 去[Nodejs官网](https://nodejs.org)下载并安装nodejs
- 本机安装好[git](https://git-scm.com/downloads)
- 将本项目克隆到本地，进入根目录执行命令`npm install`安装项目所依赖的nodejs模块

## 2、Hexo相关
大概原理，Hexo是一个基于Nodejs的静态博客生成工具，它包含了生成博客框架所需要的各种模板，具体文章内容来源于用户放置在`source/_posts`目录下的markdown文件，还有一些配置数据来源于`_config.yml`文件（内容是一种叫做YAML数据格式），最终将所有文章编译为静态的html文件到`public`目录，最后将`public`目录下的资源deploy到配置好的github仓库就可以访问了(详细原理见[Github Pages](https://pages.github.com/))

简单来说每次写文章就是新增一个`<title>.md`的markdown文件，然后将文章内容写到该文章中，最后生成静态文件发布到目标github仓库

- [Hexo介绍](https://hexo.io/zh-cn/docs/)
- `hexo new <title>.md` 新建文章
- `hexo server` 本地起一个服务，默认配置通过`localhost:4000`可以预览效果
- `hexo g --watch`：编译文件
- `hexo deploy`:发布内容 

## 3、写作相关说明
- hexo文章说明 [https://hexo.io/zh-cn/docs/writing](https://hexo.io/zh-cn/docs/writing)
- [front-matter](https://hexo.io/zh-cn/docs/front-matter)用于配置文章相关属性的字段
