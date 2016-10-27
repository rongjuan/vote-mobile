# 全栈投票项目
* 基于nodejs && express的后台服务
* 基于zepto的前端网页构建
* 前后数据分离

###注：头像上传功能暂时没加上去，用户头像都采用默认头像


## 运行项目

克隆项目

```
> $ git clone https://github.com/rongjuan/vote-mobile.git
```
在vote目录下安装依赖包

```
> $ npm install
```
启动服务器

```
> $ npm run start
```
执行完`npm run start`命令后，打开浏览器 `http://localhost:8080/vote/index`访问首页地址


## 项目说明

1. 项目需求
	- 实现投票获奖活动，票数越高，排名越高。
	- 只有报名用户才可以参加投票，每人最多投5票，每一个投票者最多只能投一票给同一个人。
	- 报名用户既是投票者，也是被投票者。
	- 用户未登入时，首页橙色按钮显示我要报名状态，点击进入报名页。
	- 用户已登入，首页橙色按钮显示个人主页，点击进入登入者的个人主页。
	- 用户未登入进行投票，点击投票则提示用户先登入或者报名才可以参与投票。
	- 首页搜索内容可以为用户的名称或编号，如有多个相同名称，则返回所有匹配名称的用户信息。
	- 搜索页的用户内容也可以进行投票，投票行为和首页的投票行为一致。
	- 首页用户信息通过上拉加载刷新进行分页，每页为十条数据。
	- 个人详细页需要显示投票者信息。


2. 页面访问地址
	- 首页：[localhost:8080/vote/index](localhost:8080/vote/index)
	- 报名页：[localhost:8080/vote/register](localhost:8080/vote/register)
	- 个人详细页：[localhost:8080/vote/detail/{id}](localhost:8080/vote/detail)
	- 搜索页：[localhost:8080/vote/search](localhost:8080/vote/search)
	- 规则页：[localhost:8080/vote/rule](localhost:8080/vote/rule)
	

	
