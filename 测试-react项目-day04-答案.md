## 1. 写出5个项目开发中常用的数组方法, 和作用
	push()/pop()/shift()/unshift()
	forEach(item => {}): 遍历数组
	filter(item => true/false): 遍历过滤返回一个子数组
	map(item => newItem): 遍历返回一个对应的新数组
	find(item => true/false): 遍历查找满足条件的第一个元素
	findIndex(item => true/false): 遍历查找满足条件的第一个元素的下标
	reduce((preTotal, item) => newTotal, initTotal): 遍历累计     [1, 3, 2, 7]


## 2. 说说你对cookie的理解(分类, 创建, 保存, 使用)
	cookie由key和value组成的文本小数据
	分类: 会话cookie和持久化cookie
	由服务器端创建: res.cookie(key, value, {maxAge: 1000})
	由浏览器端保存: 浏览器接收到新的cookie会自动保存(内存/文件)
	使用: 浏览器发送请求时自动携带对应的cookie, 服务器端通过req读取: req.cookies.key

## 3. 组件的二种分类
	1). 路由组件和非路由组件
	2). 容器组件和UI组件

## 4. src下的各个文件及其说明
	api          ajax请求后台接口
	assets        共用资源文件夹
		css
		imgages
	components   UI组件
	containers   容器组件
	redux        redux相关
		actions.js
		action-types.js
		reducers.js
		store.js
	util         工具
	index.js     入