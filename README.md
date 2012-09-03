##Pagination Actionscript 3.0 Library
基于Ember.js 0.9.8.1的jQuery Mobile“代理”插件

### 使用方法：  
依赖：  
<pre>
&lt;script src=&quot;ember-0.9.8.1.min.js&quot;&gt;&lt;/script&gt;
&lt;script src=&quot;jquery-1.8.0.min.js&quot;&gt;&lt;/script&gt;
</pre>

引入：  
<pre>
&lt;script src=&quot;ember-bridge-jqm.js&quot;&gt;&lt;/script&gt;
</pre>


使用（JavaScript）：  
<pre>
App.PageView = Mov.PageView.extend({
    templateName:'main',
    id: 'page-view',
    didInsertElement: function() {
        $.mobile.changePage(this.$());
    }
});
App.HeaderView = Mov.HeaderView.extend();
App.FooterView = Mov.FooterView.extend();
App.ContentView = Mov.ContentView.extend();
</pre>

使用（HTML）：  
<pre>
&lt;script type=&quot;text/x-handlebars&quot; data-template-name=&quot;main&quot;&gt;&lt;/script&gt;

	{{#view App.HeaderView}}
		&lt;h1&gt;Adobe Reader&lt;/h1&gt;
	{{/view}}

	{{#view App.ContentView}}
	{{/view}}

	{{#view App.FooterView}}
		&lt;h3&gt;via &lt;a href="http://www.k-zone.cn/zblog"&gt;Kenshin&lt;/a&gt;&lt;/h3&gt;
	{{/view}}

&lt;/script&gt;

&lt;div data-role=&quot;page&quot;&gt;&lt;/div&gt;
</pre>


## 参考：
* [https://github.com/LuisSala/emberjs-jqm](https://github.com/LuisSala/emberjs-jqm)
* [https://github.com/tolbard/ember-moving](https://github.com/tolbard/ember-moving)

## 更新日志：
version 1.0 [2012-8-27]
* 适合Ember.js 0.9.8.1与jQuery Mobile 1.2.0 alpha（及以下）版本
* 适合jQuery Mobile单页面模式

## 联系方式：
* 博客：[k-zone.cn](http://www.k-zone.cn/zblog)
* 微博：[新浪微博](http://weibo.com/23784148)
* 联络：kenshin[AT]ksria.com

## 版权和许可：
Copyright 2012 [k-zone.cn](http://www.k-zone.cn/zblog)  
Licensed under MIT or GPL Version 2 licenses
