# 知识库
知识库，总结在项目中实际使用的git命令，docker部署，mongodb，mysql等知识点

### git知识库
  - [git安装以及设置](git/git1.md)
  - [git的基本命令](git/git2.md)
### docker知识库
  - [基础](docker/docker.md)
### mysql数据库知识库
  - [第一天:基础]
      - [Mysql数据库基础语法](sql/mysql.md)
  - [第二天:提升练习]
      - [语法练习1](sql/mysql2_1.md)
      - [语法练习2](sql/mysql2_2.md)
  - [第三天:mysql与python交互]
      - [交互](sql/mysql3.md)
### redis知识库
  - [第一天:安装/基础]
      - [redis安装以及基础语法](sql/redis.md)
  - [第二天:订阅]
	  - [订阅](sql/redis1.md)

### mongodb知识库
  - [安装及配置](sql/mongodb.md)
  - [基础语法](sql/mongodb语法.md)

### PEP 8风格指南
  
  - [风格指南](PEP8风格指南.md)

### Django知识库
  - [第一天:环境与创建项目]
		  
        - 环境搭建: virtualenv的安装与使用,pycharm中环境的配置
        - Django概念: MVC模式/MVT模式
        - 项目创建: 创建Django工程目录，创建应用app，使用admin管理后台 
      - [django概念介绍](django/1.1django_pattern.md)
      - [virtualenv环境](django/1.2python_virtualenv.md)
      - [创建django项目](django/1.3django_halloWorld.md)
      - [admin管理](django/1.4django_admin.md)
  - [第二天:模型]
  
	    - M模型：模型的定义，字段的定义，max_length，default, null， unique等参数定义
	    - ORM对象关系映射概念，数据的迁移
	    - 数据的查询，all，filter，get等
      - [模型设计](django/2.1django_models.md)
      - [练习](django/2.2django_mysql_lianxi.md)
  - [第三天:模型加餐/模板]
  
	    - 模型设计概念：一对一，一对多，多对多的模型定义
	    - 模型设计案例：学生和学生拓展表一对一模型设计，学生和课程表多对多模型设计，学生和班级一对多模型设计
	    - 模板1：在settings.py文件中静态static的配置定义，在页面中静态文件的加载
	    - 模板2：模板中逻辑运算符，if、ifequal、forloop、for empty等
	    - 模板3：父模板中定义block块和子模板中继承与调用父模板中block块
	    - 模板4：模板中注解，注解代码的可见与不可见，三种注解的区别
	    - 模板5：模板中定义修饰变量的过滤器，使用管道符‘|’，以及Django中过滤器的自定义
	    
      - [模型关联设计](django/3.1django_model_more.md)
      - [模板](django/3.2django_temp.md)
  - [第四天:视图1]
  
	    - URL的正则匹配与带参URL和不带参URL定义
	    - 带参URL的redirect跳转与参数传递，以及页面内中URL反向解析的定义
	    - Django中DEBUG为False和True的区别,以及当DEBUG为False时，静态文件解析与错误(403、404、500)视图的定义
	    - 请求与响应：请求中属性和方法，响应中属性和方法
      - [路由/反向解析](django/4.1django_urls.md)
  - [第五天:视图2]
	    
		- 什么是会话技术，什么是HTTP无状态协议，解决HTTP无状态协议的方案----> cookie + session
		- cookie的使用：如何设置cookie，删除cookie，如何设置失效
		- session的使用：如何使用session，删除session，session中数据存储的时效。在Django中如何配置session，数据库中django_session表的使用
		- 案例1：cookie和session实现的原理
		
      - [cookies/session](django/5.1django_coo_sess.md)
      - [登录/注册--自己实现](django/5.2django_regist_login.md)
      - [登录/注册--django实现](django/5.3django_regist_login.md)
  - [第六天:插件]
		
		- 中间件middleware的工作原理，如何拦截各阶段的请求，重构拦截各阶段的方法
		- 数据分页：掌握Paginator分页的工作原理，实现分页的方式
		- 定义模型中上传文件字段，安装Pillow，定义上传文件的media路径，定义页面中如何解析media中上传图片
		- 中间件案例1： 实现登录注册功能
		- 富文本编辑器案例2： 使用富文本编辑器实现文本内容编辑，图片上传
      - [验证码/中间件/分页](django/6.1django_plug.md)
      - [文件上传](django/6.2django_media.md)
      - [kindeditor富文本编辑器](django/6.3django_kindeditor.md)
  
  - [第七天:日志/restful]

  		- setting.py中日志logging文件的配置，logging的四大组成，loggers，handlers，filters，formatters的处理流程，以及日志打印
  		- 架构设计指导原则，rest的核心定义，如何定义符合规范的api接口。资源、请求、状态码的理解。
  		- Django中restframework安装，settings.py中的定义，以及如何定义对资源的CRUD操作
      - [日志](django/7.1django_log.md)
      - [restful1](django/7.2django_restful.md)
  - [第八天:权限、角色]
	    
	    - 权限与角色的剖析，模型关联关系的定义。权限中一对多和多对多中数据的增删改查。
	    
	  - [权限、角色](django/8.1django_role_premission.md)
  - [第九天:restframework2]

	    - 重构api响应结构，api中异常响应结构重构与定义
	    - 定义虚拟化serializer，验证每一个字段的错误信息，配置参数等
	  - [响应结构/ajax-CRUD](django/9.1django_restful3.md)
  - [第十天:restframework3]
	    
 	    - api返回数据的分页配置，过滤类的定义与配置
 	    - 调用postman实现通过api对数据进行CRUD操作
 	      
	  - [分页/过滤/筛选](django/10.1django_restful4.md)
  - [第十一天到十五天：项目]
	  - [爱鲜蜂案例2班](https://github.com/coco369/axf)
	  - [爱鲜蜂案例3班](https://github.com/coco369/django-teaching-15days/tree/master/qf_1803/1.django/day09/%E4%BB%A3%E7%A0%81/axf)
	  - [爱鲜蜂案例4班](https://github.com/coco369/django-teaching-15days/tree/master/qf_1804/1.django/day14/%E4%BB%A3%E7%A0%81/axf4)
	  - [centos7部署项目](部署/centos部署.md)
	  - [ubuntu部署项目](部署/ubuntu部署.md)

### Flask知识库
  - [第一天:HelloFlask]
  
	  	- flask配置：微的定义，最小flask的web引用，虚拟环境搭建，安装flask
		- mvc概念,项目的符合MVC模式的拆分
		- 项目运行管理：flask_script库使用，debug配置等
	  - [flask简介](flask/1.0flask_helloflask.md)
	  - [flask蓝图](flask/1.1flask_blueflask.md)
  - [第二天:views]
	  
		- 请求与响应：POST/GET请求传参，类字典的区别
		-  session/cookie概念：用法，redis的配置
		-  应用案例1：使用session模拟登陆功能，装饰器的定义使用
		
	  - [flask请求与响应/错误处理](flask/2.1flask_request_response_error.md)
	  - [session/cookie](flask/2.2flask_session_cookie.md)
	  - [应用案例1：登录校验](flask/2.3flask_login.md)
	  
  - [第三天:templates与models]
  
		- 基础模板的定义，模板的继承，挖坑以及填坑。宏定义
		- 模板中逻辑控制，过滤器，以及静态static的配置
		- 模型的定义，数据库的创建，学生模型CRUD操作
		
	  - [flask-template](flask/3.1flask_templates.md)
	  - [flask-models1](flask/3.2flask_models.md)
  - [第四天:models与一对多关系]
	    
        - 深入数据库的增删改查，查询数据filter和filter_by
        - 运算符--contains、startswith、__gt__等
        - 筛选--offset、limit、get、first、paginate等
        - 逻辑运算符--and_、or_、not_
        - 模型之间的一对多的关联关系的定义
        
	  - [flask-models2](flask/4.1flask_models.md)
	  
  - [第五天:多对多关系/debugtoolbal]

	    - 模型之间的多对多的关联关系的定义，多对多的数据的CRUD
	    - 拓展库的使用：debugtoolbar，flask_restful
	    
	  - [flask-models3](flask/5.1flask_models.md)
	  - [flask-extensions](flask/5.2flask_extensions.md)
	  
  - [第六天到第10天：项目]
	  - [爱家案例](https://github.com/coco369/aj)
	  - [爱家案例2班](https://github.com/coco369/django-teaching-15days/tree/master/qf_1802/2.flask/day9/%E4%BB%A3%E7%A0%81/day06)
	  - [爱家案例3班](https://github.com/coco369/django-teaching-15days/tree/master/qf_1803/2.flask/day09/%E4%BB%A3%E7%A0%81/aj)
	  - [centos7部署项目](部署/aj_centos部署.md)
	
  - [Flask和Django区别]
	  - [区别](flask/6.0flask_django_diff.md)

### 爬虫


  - [第一天:爬虫]
		
		- 概念：爬虫的由来/用来做什么
		- 数据采集与分析：urllib/requests/bs4/mongodb/mysql/redis等
		- 请求头-反爬虫：User-Agent，Accept，Accept-Language等
		- 百度搜索：中文的编码解码
		- ssl: ssl认证
		- 应用案例1：urllib获取百度首页源代码，其中User-Agent的使用
		- 应用案例2：爬去智联上某工作某地点的岗位个数
		- 作业1：爬取智联上某工作某地点的工作名称，公司等信息
		- 作业2：爬取格言网(https://www.geyanw.com/)上的某一个模块的名言警句
		- 作业3：爬取搜狗图片中的新垣结衣的图片
	  - [爬虫引入/User-Agent讲解](spider/1.0spider_concept_urllib.md)
	  - [应用案例:爬取智联工作/百度源码](spider/1.1spider_baidu_zhilian_search.md)


  - [第二天:数据采集]
		
		- 爬取工具：requests使用、bs4使用、urllib使用
		- xpath语法、re正则表达式语法
		- 应用案例1：获取豆瓣电影中动态加载电影资源信息
		- 应用案例2:爬取知乎发现里面的提问的链接数，和链接地址
	  - [采集(bs4/requests)](spider/2.0spider_collect.md)
	  - [提取xpath/re](spider/2.2spider_re_xpath.md)
	  - [应用案例1:爬知乎的提问/豆瓣电影信息](spider/2.1spider_movies_questions.md)
	  - [应用案例2:爬取搜狐体育的新闻信息](spider/2.3spider_souhu_sports.md)

	
  - [第三天:多线程爬虫]
  
  		- 概念：线程、进程、同步、异步、并发、阻塞、非阻塞、并发、并行
	  	- 进程、线程概念：多线程定义，守护线程，线程启动
	  	- 线程锁
	  	- 应用案例1：I/O密集型，计算密集型的单线程多线程对比
	  	
	  - [并发、并行、同步、异步线程、进程](spider/3.0spider_process_threading.md)
	  - [线程锁](spider/3.1spider_threading_lock.md)
	  - [应用案例1:计算密集型和IO密集型的性能对比](spider/3.2spider_threading_IO_calc_GIL.md)
	  - [应用案例2:多线程爬虫](spider/3.3spider_threading_douban.md)
	  

  - [第四天:协程/数据持久化]
	    
 		- 迭代器、生成器的原理概念、斐波那契的实现
	  	- 协程的概念，原理，生产者-消费者的实现
	  	- 数据持久化，redis安装配置、缓存，mongodb安装配置、语法、缓存
	  	- aiohttp:异步非阻塞的

	  - [协程](spider/4.0spider_yield.md)
	  - [练习题](spider/4.1spider_yield_practice.md)
	  - [数据库持久化](spider/4.2spider_sql_engine.md)
	  - [应用案例1:使用协程爬取豆瓣电影并持久化](spider/4.3spider_async_await.md)



 - [第五天:动态解析]

		- 动态内容分析: 什么是动态内容，分析豆瓣的动态内容加载
		- javascript逆向，selenium自动化测试框架
		- 应用案例1: 使用selenium模拟登陆知乎
		- 应用案例2: 使用selenium解析豆瓣电影信息
		
	  - [动态内容解析/selenium用法](spider/5.0spider_javascript_analyst.md)
	  - [模拟登陆知乎并截图/解析豆瓣电影信息](spider/5.1spider_selenium_login_zhihu_and_douban_movies.md)

  - [第六天:验证]
		
		- 模拟登陆:请求url分析,请求参数分析，模拟登陆状态保持

		- form模拟登陆、验证码

	  - [应用案例1：模拟登陆github](spider/6.0spider_github_login.md)
	  - [应用案例2: 验证码识别](6.1spider_verifi_aliyun.md)


  - [第七天--第十天]
  
	    - scrapy框架组件，处理流程，数据持久化
	    - scrapy项目环境搭建，创建项目命令，执行启动操作，各相关文件的处理逻辑
	    - scrapy_redis分布式爬虫原理
	    
	    - 案例1：爬取起点小说网的小说分类，以及分类的url
	    - 案例2：爬取豆瓣电影的信息，并使用mongodb持久化
		- 案例3：爬取链家房源信息，并存储在csv文件
		- 案例4：爬取微博大V的粉丝数，关注，博客等信息

      - [scrapy框架的介绍以及案例1](spider/7.0spider_scrapy1.md)
      - [scrapy爬虫豆瓣信息](spider/7.1spider_scrapy2.md) 
      - [scrapy爬取链家信息](spider/code/scrapy框架/lianjiaspider)
      - [scrapy爬取微博用户信息](spider/7.2spider_weibo_scrapy3.md)
	      - [分析接口](spider/7.2spider_weibo_scrapy3.md)
	      - [分析用户信息](spider/7.3spider_weibo_scrapy_user_info.md)
	      - [分析关注信息](spider/7.4spider_weibo_scrapy_follows_info.md)
	      - [分析粉丝信息](spider/7.5spider_weibo_scrapy_fans_info.md)
	      - [IP代理池/User-Agent设置](spider/7.6spider_weibo_scrapy_ips_user_agent.md)
	  - [scrapy爬取豆瓣即将上线电影/正在热播电影信息](spider/code/scrapy框架/doubanMoviespider)
	  - [分布式爬虫](spider/7.7spider_scrapy_redis.md)

  
### Tornado知识库







