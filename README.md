# thinkjoy-frontend-file
### npm install -g hexo
### git clone ....
### npm install
### npm install hexo-deployer-git --save
### hexo n   #写文章
### hexo g   #生成
### hexo s   #本地启服务
### hexo d   #部署   


#出现账号deploy问题按下面操作

###ssh-keygen -t rsa -C "***@**" (你的github账号)
  
###会生成在你的电脑 (/home/you/.ssh/id_rsa)
    
###vim /home/you/.ssh/id_rsa  
  
###复制内容，发给sfdeng@thinkjoy.cn
  



#新建文章

###title: postName #文章页面上的显示名称，可以任意修改，不会出现在URL中
###date: 2013-12-02 15:30:16 #文章生成时间，一般不改，当然也可以任意修改
###categories: example #分类
###tags: [tag1,tag2,tag3] #文章标签，可空，多标签请用格式，注意:后面有个空格
###description: 附加一段文章摘要，字数最好在140字以内。
###---



#Hexo命令
###hexo new "postName" #新建文章
###hexo new page "pageName" #新建页面
###hexo generate #生成静态页面至public目录
###hexo server #开启预览访问端口（默认端口4000，'ctrl + c'关闭server）
###hexo deploy #将.deploy目录部署到GitHub

#常用复合命令：
###hexo d -g #生成加部署
###hexo s -g #预览加部署

#简写：
###hexo n == hexo new
###hexo g == hexo generate
###hexo s == hexo server
###hexo d == hexo deploy


#插件
###sitemap & rss
###根目录安装
### $ npm install hexo-generator-feed
### $ npm install hexo-generator-sitemap
>之后重启博客，访问/atom.xml和/sitemap.xml，会发现已经生成了。可以把sitemap提交到搜索引擎的站长平台来增加收录。
