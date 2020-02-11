---
title: "HUGO快速搭建博客"
date: 2020-02-05T13:19:27+08:00
draft: false
---
# **前言**
Hugo是Go语言实现的静态网站生成器,快速，简洁是它的特点。
这是hugo官方网站 https://gohugo.io/ ，可以通过[Quick Start](https://gohugo.io/getting-started/quick-start/)按钮快速生成你的博客。
 ![](/images/index.jpg)
# **首先你要有HUGO**
 去 [Hugo releases](https://github.com/gohugoio/hugo/releases)页面找到适合你的系统的安装程序并下载。
 我用的是windows系统，选择的是`hugo_0.63.1_Windows-64bit`
 ![](/images/install.jpg)
下载并解压，将hugo放到D:\Software\hugo\hugo.exe
**把`D:\Software\hugo\`添加到PATH**
重启终端，运行hugo version查看版本
# **搭建博客**
进入[Quick Start](https://gohugo.io/getting-started/quick-start/)，可以看到有7步需要去做，因为已经安装完成hugo，从第二步开始即可。
总体上每步的命令都很清晰，解释也很详尽。在这里把几个需要配置的点位说明一下。
## 需要进行配置的点位
1. 第二步新建项目中 `hugo new site quickstart` 命令会生成的文件夹名为quickstart，你可以自己改变成其他名称。
2. 第三步是添加一个主题。默认命令中的主题`ananke`样式比较朴素，可以去hugo提供的主题页面下载喜欢的主题。
3. 第四步中会生成你的第一篇博客，我们要做的就是更改title和draft。
![](/images/step4.jpg)
4. 第五步会给博客网址，可以访问，可以通过修改第六步中的`config.toml`中对语言，标题，主题进行配置。
![](/images/step5.jpg)

# **上传博客**
进行完上述步骤之后 先在文件夹中创建 .gitignore 忽略public文件夹，因为public文件夹是要用来提交的，分别进行git更利于保存和修改。
进入到public文件夹中单独建立git，在github中建立新的仓库：`用户名.github.io`进行git上传操作。
这样一来你的博客就可以在git中看到。若想使用其他网址方便所有人查看，可以在阿里云等购买域名并绑定到你的github中的页面。