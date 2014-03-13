xtemplate-demo
==============

[xtemplate](http://docs.kissyui.com/1.4/docs/html/guideline/xtemplate.html) 是 [KISSY]()http://docs.kissyui.com/ 中一个很强大的模板引擎，不仅支持 mustache ，还有很多扩展的功能。


一个典型的XTemplate模板实例：

	Hello {{name}}
	You have just won ${{value}}!
	{{#if data}}
	    {{#each data}}
	        {{name}}-{{xindex}}/{{xcount}}
	    {{/each}}
	{{/if}}

对应要填充的JSON：

	{
	    name:'Kissy',
	    value:'10000',
	    data:[
	        {name:1},
	        {name:2}
	    ]
	}

拼装结果：

	Hello Kissy You have just won $10000! 1-0/2 2-1/2 

为方便测试，写了一个简单的小工具。

地址：[XTtemplate 测试工具]()