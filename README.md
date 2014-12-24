# [Bootstrap Table](http://bootstrap-table.wenzhixin.net.cn)

[![Build Status](https://travis-ci.org/wenzhixin/bootstrap-table.png)](https://travis-ci.org/wenzhixin/bootstrap-table) 
[![GitHub version](https://badge.fury.io/gh/wenzhixin%2Fbootstrap-table.png)](http://badge.fury.io/gh/wenzhixin%2Fbootstrap-table)
[![Bower version](https://badge.fury.io/bo/bootstrap-table.svg)](http://badge.fury.io/bo/bootstrap-table)
[![Views in the last 24 hours](https://sourcegraph.com/api/repos/github.com/wenzhixin/bootstrap-table/.counters/views-24h.png)](https://github.com/wenzhixin/bootstrap-table)
[![Gratipay](https://img.shields.io/gratipay/wenzhixin.svg)](https://gratipay.com/wenzhixin/)
[![Donate](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=ZDHP676FQDUT6)

An extended Bootstrap table with radio, checkbox, sort, pagination, and other added features.

To get started, check out http://bootstrap-table.wenzhixin.net.cn!

## LICENSE

**NOTE:** Bootstrap Table is licensed under the [The MIT License](https://github.com/wenzhixin/bootstrap-table/blob/master/LICENSE). Completely free, you can arbitrarily use and modify this plugin. If this plugin is useful to you, you can **Star** this repo, your support is my biggest motive force, thanks.

## Bugs & Enhancements (next version)

<br/>
非常感谢原作者
<br/>
## 相对于原作者版本

<pre>
	当返回的数据不是一个数组的时候，通过自身处理本身比较复杂.如 
	{
		status : 200,
		data : {
			rowcount : 300,
			resp : [ {..},{..}]]
		}
	}
</pre>
 
 * 把默认的语言改为中文了，其他语言基本上没用到,减少一个js的引用
 
 * 增加 data-page-items 属性
   
   显示数据所对应的位置，如上面的例子显示：data.resp
 	
 * 增加 data-page-row-count 属性
 	
    显示所有的列总数数据所对应的位置，如上面的例子显示：data.rowcount
 	
 * 增加 data-page-extra 属性
 	
	如果在查询的时候需要加入其他参数，而pageNumber,pageSize等参数我不想做任何改变。
	可以调用函数来获得其他的参数输入。

<pre>
		data-page-extra = "queryArgs"
		
		/*
		 * base 为系统提交之前所有的参数集合，这个地方你可以覆盖原有的任何参数
		 *
		 */
		function queryArgs(base) {
		    return {
		    	'type' : 200,
		    	'time' : 'now'
		    };
		}
</pre>



## Features

* Created for Bootstrap 3 (Bootstrap 2 supported)
* Responsive web design
* Scrollable Table with fixed headers
* Fully configurable
* Via data attributes
* Show/Hide columns
* Show/Hide headers
* Get data in JSON format using AJAX
* Simple column sorting with a click
* Format column
* Single or multiple row selection
* Powerful pagination
* Card view
* Localization

## How to get it

### Manual download

Use [Releases page](https://github.com/wenzhixin/bootstrap-table/releases) or [the source](https://github.com/wenzhixin/bootstrap-table/archive/master.zip).

### Bower

```
bower install bootstrap-table
```

### CDN

You can source bootstrap-table directly from a CDN like [CDNJS](http://www.cdnjs.com/libraries/bootstrap-table) or [bootcss](http://open.bootcss.com/bootstrap-table/).

## Reporting issues

Please provide jsFiddle when creating issues!

It's really saves much time. Use this as template:

[jsFiddle Bootstrap Table](http://bootstrap-table.wenzhixin.net.cn/examples/#basic)

Your feedback is very appreciated!

## Acknowledgements

Thanks to everyone who have given feedback and submitted pull requests. A list of all the contributors can be found [here](https://github.com/wenzhixin/bootstrap-table/blob/master/CONTRIBUTORS.md).

## Release History

Look at the [Change Log](https://github.com/wenzhixin/bootstrap-table/blob/master/CHANGELOG.md)

## Local build

To build bootstrap-table locally please run:

```
grunt build
```

Result will appear in `dist` directory.

