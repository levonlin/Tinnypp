##Tinnypp

###About

This is a clean theme for [hexo](https://github.com/hexojs/hexo)

It is based on [Tinny](https://github.com/zhanglun/hexo-theme/tree/master/Tinny).

I have made some optimizations on Tinny and you can see the [demo](http://levonlin.github.io/Tinnypp/).

###Installation

####Install

```	
	$ cd themes
	$ git clone git@github.com:levonlin/Tinnypp.git
```

####Enable

Modify the `theme` setting in `_config.yml` of the blog folder.

```
    theme: Tinnypp
```

####Update

```
	$ cd themes/Tinnypp
	$ git pull
```

###Configuration

Modify settings in the file `Tinnypp/_config.yml`.

Tinnypp :

1.uses [swiftype](https://swiftype.com/) as a site's search engine.If you want to use swiftype,please change the last `<script></script>` tag to your swiftype install code in `Tinnypp/layout/_partial/head.ejs`. (For more details, you can read [this article](http://www.jerryfu.net/post/search-engine-for-hexo-with-swiftype.html))

2.has set /atom.xml as an rss source.To use rss,you can install hexo rss plugin

```
	$npm install hexo-generator-feed
```

Then add 

```
	plugins:
	- hexo-generator-feed
```

in `_config.yml` of the blog folder.

3.get pictures for icon or avatar from `Tinnypp/source/img`. Pay attention to the sizes and formats of your pictures, the detailed configs are in `_config.yml` of the theme folder. 

For more details, you can vist [My blog](http://www.levonlin.info/tags/Tinnypp/) .And if you have any problems, you can create [issues](https://github.com/levonlin/Tinnypp/issues).

##中文说明

###关于

本主题是一个[hexo](https://github.com/hexojs/hexo)的小清新主题。就是在[Tinny](https://github.com/zhanglun/hexo-theme/tree/master/Tinny)基础上做了些我自己认为的优化（折腾）。具体效果可见[demo](http://levonlin.github.io/Tinnypp/)。

###装载本主题

####安装

```
	$ cd themes
	$ git clone git@github.com:levonlin/Tinnypp.git
```

####载入

去你博客目录下的`_config.yml`文件编辑`theme`设定如下：

```
    theme: Tinnypp
```

####升级

```
	$ cd themes/Tinnypp
	$ git pull
```

###设置本主题

编辑`Tinnypp/_config.yml`文件即可。

本主题:

1.使用[swiftype](https://swiftype.com/)作为站内搜索引擎，如果你想使用这个酷炫的搜索，请在`Tinnypp/layout/_partial/head.ejs`里将最后一个`<script></script>`标签改为你的swiftype安装代码。（具体细节可参见[这篇文章](http://www.jerryfu.net/post/search-engine-for-hexo-with-swiftype.html)）

2.使用[多说](http://duoshuo.com/)作为评论系统，可在`Tinnypp/_config.yml`中开启或关闭。此外如果你想显示评论者的[user agent](http://zh.wikipedia.org/wiki/%E7%94%A8%E6%88%B7%E4%BB%A3%E7%90%86)，可直接修改`themes/Tinnypp/layout/_partial/after_footer.ejs`里的`ds.src = '//static.duoshuo.com/embed.js';`为`'ds.src = '<%- config.root %>js/embed.js'';`，并在你的多说里添加这个[自定义css](https://github.com/levonlin/Tinnypp/blob/master/source/css/%E5%A4%9A%E8%AF%B4%E8%87%AA%E5%AE%9A%E4%B9%89.css)即可。若还想显示你的“博主头衔”，请记得编辑`Tinnypp/source/js/embed.js`里的`e.user_id == your duoshuo ID`。

3.已经设置/atom.xml为rss源。要使用rss,先安装hexo的rss插件：

```
	$npm install hexo-generator-feed
```

然后添加 

```
	plugins:
	- hexo-generator-feed
```

到博客目录下的`_config.yml`。

4.中文显示在博客目录下的`_config.yml`设置

```
	language: zh-CN
```

即可。但若想在文章发布日期有符合中文习惯的显示，请在`_config.yml`里继续设置

```
	month_format: YYYY年 MMM
	date_format: YYYY年 MMM D日 
	time_format: H:mm:ss
```

5.如果想用主题里的highgLight.js自定义代码高亮，有几点需要注意的：

* 得先把hexo的`_config.yml`（不是主题里那个）里的highlight配置为false，否则就只能用hexo自带的的代码高亮；
* 上一步做好后还得先hexo clean、再hexo g；新设置才会生效；
* 由于主题里的highgLight.js使用了cdn加载样式，自定义的代码高亮只有在联网时才会显示，同时高亮样式的名字应该参考[cdn上的](http://www.bootcdn.cn/highlight.js/)；
* highgLight.js**不支持**显示行号。

6.图标和头像的图片统一放置于`Tinnypp/source/img`。还要注意图片的格式与大小，详见主题目录的`_config.yml`。

更多细节，各位亲们可以访问[我的博客](http://www.levonlin.info/tags/Tinnypp/)。如果觉得这个主题有什么值得吐槽和改进的地方，也欢迎各位亲们给我发[issues](https://github.com/levonlin/Tinnypp/issues)。
