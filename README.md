

# NodeJs+MongoDB+jQuery+Bootstrap 搭建的豆瓣电影网站


### 基于Nodejs的练手项目
> 技术栈 Node.js + Express + MongoDB + Jade + Bootstrap + jQuery + gulp


####   项目前端搭建:
* 使用jQuery和Bootsrap完成网站前端JS脚本和样式处理；
* 前后端的数据请求交互通过Ajax完成；
* 引入了Moment.js格式化前端页面显示时间；
#### 项目后端搭建:
* 使用NodeJs的express框架完成电影网站后端搭建；
* 使用mongodb完成数据存储，通过mongoose模块完成对mongodb数据的构建；
* 使用jade模板引擎完成页面创建渲染；
* 使用Moment.js格式化电影存储时间；
#### 本地开发环境搭建:
* 使用gulp集成jshint对JS语法检查，加入browser-sync与nodemon，实现实时刷新及服务器的自动重启等功能。
#### 网站整体功能:
网站正常访问无需管理员权限，对电影的评论，需要用户登录，对网站数据的修改添加删除需要管理员的权限(role > 10)，具体功能如下：
* 实现了用户的基本注册，登录，登出及管理功能；
* 实现了搜索功能，模糊关键字可搜索电影名字及电影类别下的电影；
* 用户登录做session处理；
* 用户可以对电影进行评论；
* 电影添加分类及录入，数据可以同步豆瓣ID；
* 对电影数据作分页处理，分页查询数据库数据；
* 管理员可以对网站数据进行增加删除修改；
* 管理员可从后台查看所有的电影、用户、评论、访问量等数据；
### 网站整体效果
-------

<div>
  <img src="http://ov1nop9io.bkt.clouddn.com/FireShot%20Pro%20Screen%20Capture%20%23001%20-%20%27%E8%B1%86%E7%93%A3%E7%94%B5%E5%BD%B1%27%20-%20localhost_3000.png" width="45%" float"left" height="700" alt="电影首页"/>
  <img src="http://ov1nop9io.bkt.clouddn.com/FireShot%20Pro%20Screen%20Capture%20%23005%20-%20%27%E8%B1%86%E7%93%A3%E7%94%B5%E5%BD%B1%20%E9%9B%B7%E7%A5%9E3%EF%BC%9A%E8%AF%B8%E7%A5%9E%E9%BB%84%E6%98%8F%27%20-%20localhost_3000_movie_59fd779cfbc5b61494a80cfd.png" width="45%" float"left" height="700" alt="详情页"/>
</div>
<div text-align="center">
  <img src="http://ov1nop9io.bkt.clouddn.com/FireShot%20Pro%20Screen%20Capture%20%23007%20-%20%27%E8%B1%86%E7%93%A3%E7%94%B5%E5%BD%B1%E5%90%8E%E5%8F%B0%E5%BD%95%E5%85%A5%E9%A1%B5%27%20-%20localhost_3000_admin_movie_new.png" width="45%" alt="后台"/>
  <img src="http://ov1nop9io.bkt.clouddn.com/FireShot%20Pro%20Screen%20Capture%20%23006%20-%20%27%E5%88%97%E8%A1%A8%E9%A1%B5%E9%9D%A2%27%20-%20localhost_3000_admin_movie_list.png" width="45%" alt="后台"/>
</div>

### 运行环境
```javascript
git clone git@github.com:chenjun1127/Movie-Site.git
cd movie-site
```

> $ bower install

> $ npm install

> $ gulp


### 项目结构
``` bash
├─app
│  ├─controllers
│  ├─middleware
│  ├─models
│  ├─schemas
│  └─views
│      ├─includes
│      └─pages
├─config
├─public
│  ├─js
│  ├─libs
│  │  ├─css
│  │  │  ├─include
│  │  │  └─movie
│  │  ├─images
│  │  │  ├─includes
│  │  │  └─movie
│  │  └─scripts
│  │      └─js
│  │          ├─include
│  │          ├─movie
│  │          └─user
│  ├─sass
│  │  ├─.sass-cache
│  │  │  ├─07f2acd7c6896fe42d4498c5cc289a2d62daba74
│  │  │  ├─3a7bc1cae12d57c9fe265cae17c70ffa9f3515d8
│  │  │  ├─702ebcbe7156983bcb6a0ccee58b359ec4906e65
│  │  │  └─d865922842592340a08ca21fab8235f88832aa1c
│  │  ├─include
│  │  └─movie
│  └─upload
│      ├─movie
│      └─music
└─test
    └─user
```

