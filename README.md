## Hexo 主题 yilia-plus

## 开始使用

#### 1、安装

```
cd ./themes/
git clone --depth=1 https://github.com/JoeyBling/hexo-theme-yilia-plus.git ./yilia-plus
```

#### 2、配置

修改hexo根目录下的 `_config.yml` ![arrow_right](https://github.githubassets.com/images/icons/emoji/unicode/27a1.png) `theme: yilia-plus`

#### 3、更新

```
cd themes/yilia-plus
git pull
```

## 四、配置

  主题配置文件在主目录下的`_config.yml`，请根据自己需要修改使用。

> 完整配置Demo例子，可以参考[yilia-plus博客备份](http://github.com/JoeyBling/yilia-plus-demo)

```
# Header-菜单 配置后再_post中的md文件中填入对应的tags即可，比如
#tags:
#  - 其他
menu:
  主页: /
  日记本: /tags/日记本/
  我的导航: http://dh.jiang7zzz.xyz/
  心情随笔: /tags/心情随笔/
  韶华追忆: /tags/韶华追忆/
  技术分享: /tags/技术分享/
  网盘域名: /tags/网盘域名/
  科学上网: /tags/科学上网/
  博客网站: /tags/博客网站//
  其他: /tags/其他/

# subNav-子导航
subNav:
  github: "#"
  #gitee: "#" # 码云
  #jianshu: "#" #简书
  #cnblog: "#"
  #blog: "#"
  csdn: "#"
  #rss: "#"
  #zhihu: "#"
  #qq: "img/2434387555.jpg"
  #weixin: "img/weixin_.png"
  #weibo: "#"
  #douban: "#"
  #segmentfault: "#"
  #bilibili: "#"
  #acfun: "#"
  #mail: "mailto:zhousiwei0911@qq.com"
  #facebook: "#"
  #google: "#"
  #twitter: "#"
  #linkedin: "#"

#配置副标题相关内容,如果还不显示,看下\layout\_partial\left-col.ejs中是否被注释掉
subtitle: The first step is as good as half over.
description: description
author: JWSingle
email: 2314857815@qq.com
keywords: "linux、oracle"

# 悬停预览图片效果
hover_effect:
  ## `global` 0: Set separately, 1: Enable global 2: Close global
  ## `global` 0: 分开设置, 1: 全局启用, 2: 全局关闭
  global: 2
  # SubNav-导航
  subNav: true

# RSS订阅(关于如何配置启用:https://www.jianshu.com/p/2aaac7a19736)
rss: /atom.xml

# 是否需要修改 root 路径
# 如果您的网站存放在子目录中，例如 http://yoursite.com/blog，
# 请将您的 url 设为 http://yoursite.com/blog 并把 / 设为 /blog/。
# 新版本已弃用，请在博客根目录文件进行配置
# root: /

# Content

# 文章太长，截断按钮文字(在需要截断的行增加此标记：<!--more-->)
excerpt_link: more
# 文章卡片右下角常驻链接，不需要请设置为false
show_all_link: '展开全文'
# 数学公式
mathjax: false

# Open link in a new tab | 是否在新窗口打开链接
open_in_new:
  article: true  # 文章链接
  menu: true   # 导航菜单
  subNav: true  # 子菜单

# 打赏
# 打赏type设定：0-关闭打赏； 1-文章对应的md文件里有reward:true属性，才有打赏； 2-所有文章均有打赏
reward_type: 2
# 打赏wording
reward_wording: '谢谢你请我吃糖果'
# 支付宝二维码图片地址，跟你设置头像的方式一样。比如：/assets/img/alipay.jpg
alipay: /img/alipay.jpg
# 微信二维码图片地址
weixin: /img/weixin.png

# 目录
# 目录设定：0-不显示目录； 1-文章对应的md文件里有toc:true属性，才有目录； 2-所有文章均显示目录
toc: 1
# 根据自己的习惯来设置，如果你的目录标题习惯有标号，置为true即可隐藏hexo重复的序号；否则置为false
toc_hide_index: true
# 目录为空时的提示
toc_empty_wording: '目录，不存在的…'

# 是否有快速回到顶部的按钮
top: true

# Miscellaneous
# 百度统计
baidu_analytics: ''
google_analytics: ''

# 网站图标
favicon: /favicon.ico

# 你的头像url
avatar: /img/touxiang.jpg

# 是否开启分享
share_jia: true

# 评论：1、畅言；2、Disqus；3、Gitment；4、Giteement
# 不需要使用某项，直接设置值为false，或注释掉
# 具体请参考wiki：https://github.com/JoeyBling/hexo-theme-yilia-plus/wiki

# 1、畅言
changyan_appid: false
changyan_conf: false

# 2、Disqus 在hexo根目录的config里也有disqus_shortname字段，优先使用yilia-plus的
disqus: false

# 3、Gitment----基于GitHub的评论系统(关闭请设置gitment_owner为false)
# 关于如何集成:https://www.jianshu.com/p/ac7658cc912f
gitment_owner: false      #你的 GitHub ID
# 是否使用官方js(false可以提升访问速度，本地修改过一部分的js，官方js可能会出现服务器不稳定，不太建议使用)
gitment_remote: false
gitment_repo: ''          #存储评论的 repo name(需要在Github创建)
gitment_oauth:
  client_id: ''           #client ID
  client_secret: ''       #client secret

# 4、Giteement----【国内用户建议使用这个，相对比较快】
# 关于如何集成:https://www.jianshu.com/p/f5c4633524c7
# 基于码云的评论系统(https://gitee.com/zhousiwei/giteement)
giteement:
  enable: false  # 是否启用码云评论系统
  # 是否使用官方js(false可以提升访问速度)
  remote: false
  redirect_uri: ''   # 应用回调地址(请和配置的第三方应用保持一致)
  # 不能更改(网上开源项目`https://github.com/Rob--W/cors-anywhere`作者提供的专门用来跨域服务器的配置)
  oauth_uri: https://cors-anywhere.herokuapp.com/https://gitee.com/oauth/token
  giteeID: ''  # 你的码云账号英文名
  # 存储评论的 repo name(需要在码云仓库创建公开仓库)
  repo: ''
  gitment_oauth:
    client_id: ''           #client ID
    client_secret: ''       #client secret

# 访问量统计功能(不蒜子)
busuanzi:
  enable: true
  site_visit: true  # 站点访问量显示
  article_visit: true  # 文章访问量显示

# 网易云音乐插件
music:
  enable: false
  # 播放器尺寸类型(1：长尺寸、2：短尺寸)
  type: 2
  #id: 1334445174  # 网易云分享的音乐ID(更换音乐请更改此配置项)
  autoPlay: true  # 是否开启自动播放
  # 提示文本(关闭请设置为false)
  text: '这似乎是首纯音乐，请尽情的欣赏它吧！'

# 页面点击小红心
clickLove:
  # (关闭请设置为false)
  enable: true

# GitHub Ribbons(https://github.blog/2008-12-19-github-ribbons/)
github:
  # (关闭请设置为false)
  url: false

# 页脚 Litten(此配置项已弃用)
# 帮助我们让更多人可以更方便使用Hexo，请尽量不要修改此主题配置
pageFooter:
  jack: GitHub:<a href="xxx1" target="_blank"></a>

# 开启百度站长平台自动推送(https://ziyuan.baidu.com/linksubmit/index)
baidu_push: false

# 版权声明
# 版权声明type设定：0-关闭版权声明； 1-文章对应的md文件里有copyright: true属性，才有版权声明； 2-所有文章均有版权声明
copyright_type: 2
# 版权声明自定义文本(关闭请设置为false)
copyright_text:

# 网站成立年份(默认为 2018，若填入年份小于当前年份，则显示为 2018-2019 类似的格式)
since: 2018

# Progress Bar | 页面加载进度条
# Demo: http://github.hubspot.com/pace/docs/welcome/
# type: barber-shop|big-counter|bounce|center-atom|center-circle|
#       center-radar|center-simple|corner-indicator|flash|flat-top|
#       loading-bar|mac-osx|minimal
# color: black|blue|green|orange|pink|purple|red|silver|white|yellow|
progressBar:
  enable: false
  type: 'minimal'  # Keep Quotes | 保留引号避免出错(某些type会导致样式重叠排版错误)
  color: blue

# Apple Touch icon 苹果图标(关闭请设置为false)
apple_touch_icon: '/apple-touch-icon-180x180.png'

# Tab Title Change | 标签页标题切换
tab_title_change:
  enable: false
  left_tab_title: '(つェ⊂) 我藏好了哦~ '
  return_tab_title: '(*´∇｀*) 被你发现啦~ '

# https://github.com/willin/hexo-wordcount
# 是否开启字数统计(关闭请设置enable为false)
# 也可以单独在md文件里Front-matter设置`no_word_count: true`属性，来自定义关闭字数统计
word_count:
  enable: true
  # 只在文章详情显示(不在首页显示)
  only_article_visit: true

# 文字输入特效
# https://github.com/disjukr/activate-power-mode
activate_power_mode:
  enable: true
  # 使输入模式丰富多彩
  colorful: true
  # 是否开启摇动
  shake: false

# 飘雪特效
# https://github.com/MlgmXyysd/snow.js
snow: false

# 看板娘动态模型插件
## https://github.com/JoeyBling/live2d-widget.js
live2d:
  # (关闭请设置为false)
  enable: false
  # 模型名称(取值请参考：https://github.com/JoeyBling/hexo-theme-yilia-plus/wiki/live2d%E6%A8%A1%E5%9E%8B%E5%8C%85%E5%B1%95%E7%A4%BA)
  model: hibiki
  display:
    position: right # 显示位置：left/right(default: 'right')
    width: 145  # 模型的长度(default: 150)
    height: 315 # 模型的高度(default: 300)
    hOffset: 50 # 水平偏移(default: 0)
    #vOffset: -20 # 垂直偏移(default: -20)
  mobile:
    show: false # 是否在移动设备上显示(default: true)
    scale: 0.6 # 移动设备上的缩放(default: 0.5)
  react:
    opacity: 0.8 # 模型透明度(default: 0.7)

# 样式定制 - 一般不需要修改，除非有很强的定制欲望…
style:
  # 头像上面的背景颜色
  # header: '#D3D1DC'
  header: '#4d4d4d'
  gif:
    # 是否启用左侧边栏动态图效果
    enable: false
    # 自定义背景图路径(默认可以不设置，提供默认背景图)
    # path: /img/biubiubiu.gif
  # 右滑板块背景
  slider: 'linear-gradient(200deg,#a0cfe4,#e8c37e)'

# slider的设置
slider:
  # 是否默认展开tags板块
  showTags: true

# 智能菜单
# 如不需要，将该对应项置为false
# 比如
#smart_menu:
#  friends: false
smart_menu:
  innerArchive: '所有文章'
  friends: '友链'
  aboutme: '关于我'

# 友情链接
friends:
  技术笔记:  #网站名称
    #网站地址
    url: https://zhousiwei.gitee.io/ibooks/
    #网站图片(可忽略不写)
    img: https://zhousiwei.gitee.io/ibooks/favicon.ico
    #网站简介(可忽略不写)
    description: 记录工作和学习过程中的笔记：Java、前端开发、Hexo博客、聚合支付、Linux笔记、ElasticSearch、ELK日志分析
  GitHub:
    url: https://github.com/JoeyBling
  CSDN:
    url: https://blog.csdn.net/qq_30930805

# 关于我
aboutme: xxx

```

### 注意：

- **hexo 的 CNAME 文件** 需要放在source 目录下，每次运行hexo clean会清除public 目录，hexo g重新生成，hexo d发布到远程服务器。

1、准确来说 CNAME 文件是放在 hexo 项目下的 source 目录，你再运行下

```text
hexo generade
```

然后你再去 public 目录中看看就明白了

BTW，为了达到更有说服力的验证，最好在开始前先运行下

```text
hexo clean
```

这样会先删除 public 目录

- **hexo 的 README.md等文件**

  [原文]: (https://www.dazhuanlan.com/2020/03/20/5e73a3d07ebbc/)

  文件添加在 **Hexo**目录下的**source**根目录下创建**README.md**文件。并编辑保存。

  - **防止README.md被渲染**

  编辑**Hexo**目录的_config.yml文件中的“skip_render”参数。
  eg：

  ```
  skip_render: [README.md]
  ```

  保存并退出。

  - **完成**

  试着命令部署，再去你的 Git仓库看看是否存在README.md文件。

  ```
  $ Hexo clean && hexo g && hexo d
  ```

- **md中存在<title>标签时《所有文章》功能主页时不生效，模板开发者暂未解决【待解决】**