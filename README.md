# thinkjoy-frontend-file
### npm install -g hexo
### npm install
### npm install hexo-deployer-git --save
### hexo n   #写文章
### hexo g   #生成
### hexo s   #本地起服务
### hexo d   #部署       与hexo g合并为  hexo d -g


###出现账号deploy问题按下面操作

  ssh-keygen -t rsa -C "***@**" (你的github账号)
  
  会生成在你的电脑 (/home/you/.ssh/id_rsa)
    
  vim /home/you/.ssh/id_rsa  
  
  复制内容，发给sfdeng@thinkjoy.cn
  



### 新建文章

  title: postName #文章页面上的显示名称，可以任意修改，不会出现在URL中
  
  date: 2013-12-02 15:30:16 #文章生成时间，一般不改，当然也可以任意修改
  
  categories: example #分类
  
  tags: [tag1,tag2,tag3] #文章标签，可空，多标签请用格式，注意:后面有个空格
  
  description: 附加一段文章摘要，字数最好在140字以内。
  
  ---

