
### AwooMD-方便发布博客文章的markdown编辑器

#### 功能介绍

- 实时预览
- 自带markdown各种标签，即使不懂语法，也能轻易完成编辑
- 支持流程图，时序图等
- 生成hexo等静态博客文章模板
- 上传服务器后自动生成博客站点，并提交GitHub Pages
- 跨平台

> 注意事项：新建的hexo模板文章默认保存在hexo目录下的source/_posts目录下，以便发布！

#### 快速新建Hexo文章模板

- hexo文章与普通的markdown格式有些差异

```
---
title: hexo模板
tags:
	- linux
categories:

---

```


#### 准备环境
- 目前仅支持Windows7+ 系统- Hexo功能正常- Git ssh key免密码登录
#### 准备环境配置教程> 如果是老司机，准备环境没问题则跳过此步骤
- 安装和配置Git
	- [官方下载](https://git-for-windows.github.io/ "官方下载")并安装Git客户端	- 开始配置ssh key，参考[Windows 7下Git SSH 创建Key的步骤](http://blog.csdn.net/lsyz0021/article/details/52064829 "Windows 7下Git SSH 创建Key的步骤")
- 安装nodejs
	- [官方下载](http://nodejs.cn/download/ "官方下载")并安装nodejs
- 使用npm安装Hexo
	- 国内安装可能会出现问题，建议先安装cnpm命令	`npm install -g cnpm --registry=https://registry.npm.taobao.org`
	- 在执行安装Hexo命令	`cnpm install hexo-cli -g`
	- 新建进入hexo目录，右键Git Bash Here执行命令	`git clone git@git.coding.net:ccw55/ccw55.git`
	- 打开hexo配置文件`_config.yml`	修改	```		deploy:		  type: git		  repository: #你自己的git ssh提交路径		  branch: master	```	其他修改设置，请参考[hexo配置](https://hexo.io/zh-cn/docs/configuration.html "hexo配置")	- 到此环境就准备好了
#### AwooMD使用教程
- 下载安装
- 设置Hexo目录
- 编写md文章
- 预览并完成部署
------------------------

将hexo打包进软件包内

实现自动保存保存打开记录


