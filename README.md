# easyUtil_ImgPreview
  图片预览及操作插件
<h3>简介</h3>
		<h4>&emsp;&emsp;原生js实现图片预览及回调函数操作功能插件，可以拖拽或通过input文件上传功能实现图片预览，自动筛查图片类型，可提示非图片类型数量，并调用回调函数</h4>
		<h4>&emsp;&emsp;支持模块化引用</h4>
		<h4>&emsp;&emsp;1.0版本为普通递归函数调用，无兼容性问题；2.0版本为Promise加生成器函数优化版本，已完成转ES5兼容处理</h4>
		<h3>API:</h3>
		<h3>入口</h3>
		<ul>
			<li>普通调用全局引用名称为easy_ImgPre，模块化可自定义名称</li>
		</ul>
		<h3>具体方法及参数（以普通调用名称为例）</h3>
		<ul>
			<li>
				以如下方法初始化即可：<br/>
				&emsp;&emsp;easy_Calendar.init({<br/>
				&emsp;&emsp;&emsp;&emsp;main_id ： ""，必填项，显示图片的容器及拖拽区域id，如只写这一项，则启用拖拽功能； <br/>
				&emsp;&emsp;&emsp;&emsp;input_id ：""，选填，使用input文件表单标签的id，如填写这一项，则启用input表单上传功能；<br/>
				&emsp;&emsp;&emsp;&emsp;multiple ：true，选填，预览图片是否累加显示，默认true, 如不需要累加，设为false，则每次只显示当前操作图片；<br/>
				&emsp;&emsp;&emsp;&emsp;two_methods ：false，选填，是否启用拖拽和input双功能预览， 默认只启动一种，如果填写true，则两种方式都启动，且input_id为必填项；<br/>
				&emsp;&emsp;&emsp;&emsp;fn ：选填，图片预览后回调函数，默认无，可自定义，传入参数为files，包含最近一次操作的纯图片文件数组。<br/>
				&emsp;&emsp;})<br/>
			</li>
		</ul>
		<h4>兼容性：支持FileReader的浏览器测试均兼容</h4>
