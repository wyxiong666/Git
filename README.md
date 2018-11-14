# Git 上传使用心得
##1.git配置
   >config --global user.name "你的用户名"
   >git config --global user.email "你的邮箱"
    git config --list 检查你的邮箱和用户名是否配置成功了

##2.创建本地git仓库
   新建文件夹:test 也可以已经写好的
   >cd test 进入文件
   git init (初始化本地git仓库) 这步很重要的哎，切记！！！

##3.推送到远程仓库
   >git add .  (.意思把全部文件进行推送)

##4.添加到暂存区
   >git commit -m "备注信息，方便以后查询和他人查看"

##5.与远程仓库关联:
   >git remote add origin https://github.com/wyxiong666
    查看关联远程仓库地址:git remote -v
   删除关联的远程仓库：git remote rm origin

##6.把远程仓库里的内容先拉一下,避免发生冲突哎
   >git pull --rebase origin master

##7.最后push就好了(第一次加-u 以后再push可以不写啦)
   >git push -u origin master

###最后感谢廖雪峰 https://www.liaoxuefeng.com
