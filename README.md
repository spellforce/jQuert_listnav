# jQuery ListNav [![Travis Build](https://travis-ci.org/esteinborn/jquery-listnav.png?branch=master)](https://travis-ci.org/esteinborn/jquery-listnav) [![Built with GruntJS](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com)

> jQuery ListNav will add a slick "letter-based" navigation bar to all of your lists. Click a letter to quickly filter the list to show items that match that letter.

[View the ListNav Demo](http://esteinborn.github.io/jquery-listnav)

### Install using Bower

`bower install jquery-listnav`

## Manual Install
#### Insert into &lt;Head&gt;:
<pre><code>&lt;link rel="stylesheet" href="listnav.css"&gt;</code></pre>

#### Code up your list:
<pre><code>&lt;ul id="myList"&gt;...&lt;/ul&gt;</code></pre>

#### Insert before &lt;/body&gt;:
<pre><code>&lt;script src="jquery-listnav.min.js"&gt;&lt;/script>
&lt;script&gt;
	$("#myList").listnav();
&lt;/script&gt;</code></pre>

#### Navigation:

The navigation defaults to being placed directly above your list element. You can place the navigation in a place of your choice by adding to your markup.

<pre><code>&lt;div id="{myList}-nav"&gt;&lt;/div&gt;</code></pre>

## Options
<pre><code>$("myList").listnav ({
initLetter: '',//筛选到特定字母在初始化列表 ('a'-'z' '-' [数字 0-9]，'_' [其它])
includeAll: true,//包括所有按钮
includeOther: false, // 包括 '...' 选项来过滤非英语字符的
includeNums: true,//包括"0-9 的过滤选项
flagDisabled: true,//'ln-禁用' 类添加没有要显示内容的导航项目
removeDisabled: false,// 删除那些 'ln-禁用' 导航项目 (flagDisabled 必须设置为 true 为此功能)
allText: 'All',//在导航栏到所有按钮设置自定义文本
noMatchText: '没有内容', // 设置自定义文本没有要显示内容的导航项目
showCounts: true, //显示匹配以上鼠标的那封信的列表项的数目
dontCount: '', // 的逗号分隔列表选择您想要排除在计数函数 (导航上的数字)
cookieName: null,// 将此设置为一个字符串，以记住最后一个单击的导航项目需要 jQuery 插件 Cookie ('myCookieName')
onClick: null,// 设置当您单击导航项时将触发的函数。看看演示 5
prefixes: [],  // 设置数组应该算是有前缀和第一个字前在前缀后的前缀: ['' 'a'、 '我']
filterSelector:'' // 将筛选器设置为一个 CSS 选择器，而不是每个项目的第一个文本字母
});</code></pre>

# Showcase

The following websites are currently using ListNav to filter their lists:

[Santa Fe College](http://www.sfcollege.edu/az/)
