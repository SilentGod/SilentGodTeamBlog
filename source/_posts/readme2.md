title: readme2
date: 2015-07-17 01:04:10
tags:
---

作为新手GIT安装和远程库推送，廖老撕讲得很清晰，安装、创建版本库、时光机和远程仓库一定要看。


在开始下面步骤之前，要连接好team的仓库，能够实现从本地向远程推送，连接方法参照廖老撕的远程仓库克隆。

博客更新步骤
初始条件：已安装 git、node.js 
（对于windows用户可以使用git bash(baidu msysgit)，node.js(baidu 它的官网 下载install版本) hexo在此时还没有装载，稍后我们通过git安装它）


1.将该仓库更新拉回本地：
 git pull 
如果尚未克隆到本地，则执行：
 git clone git@github.com:SilentGod/SilentGodTeamBlog.git 
node.js会自动配置用户和系统环境变量，自己不要乱改，我改了一下，后面的操作马上就显示找不到文件。。。。

2.hexo 程序安装 

打开git 
i.切换到博客文件夹（SilentGodTeamBlog）：  
$cd SilentGodTeamBlog （如果仓库不在第一级目录，那么多cd几次，找到.git）
ii.安装： 

 $npm install -g hexo
 这时候会显示很多目录横线，开头有WARN

 $hexo init
 INFO copying data to ~
 you almost done!

 $hexo d -g

 成功了~



3.修改博客内容
◦修改文章： a.打开source/_post文件夹下的md文章文件，修改，保存。
b.发布： a.切换到博客文件夹
b.使用 hexo d -g 命令发布。

（具体操作）在git中 $cd 到_posts目录下 ，git add ,cat,commit ,git push origin master成功修改 ,hexo d -g 成功发布）


◦添加文章： a.切换到博客文件夹
b.生成博客文件：  hexo new 文章标题 
c.打开source/_post文件夹下相应的md文章文件，修改，保存。
d.发布
（具体操作）在git中，hexo new 文件名（不需要加.md）,然后 add commit push hexo d-g,成功发布~


4.提交更新内容（务必不要忘记）：
i. git add . 
ii. git commit -m "修改描述" 
iii. git push origin master 

 
   

Status
 API
 Training
 Shop
 Blog
 About
 Help
 