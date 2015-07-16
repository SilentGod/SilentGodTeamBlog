# SilentGodTeamBlog

## 博客更新步骤
1. 将该仓库更新拉回本地：    
  ```git pull```    
  如果尚未克隆到本地，则执行：  
  ``` git clone git@github.com:SilentGod/SilentGodTeamBlog.git ```

2. hexo 程序安装    
  ``` npm install ```

3. 修改博客内容
  - 修改文章：
    1. 打开source/_post文件夹下的md文章文件，修改，保存。
    2. 发布：
      1. 切换到博客文件夹（SilentGodTeamBlog）： ``` cd SilentGodTeamBlog ```
      2. 使用```hexo d -g```命令发布。
  - 添加文章：
    1. 切换到博客文件夹
    2. 生成博客文件： ```hexo new 文章标题```
    3. 打开source/_post文件夹下相应的md文章文件，修改，保存。
    4. 发布

4. 提交更新内容（务必不要忘记）：
  1. ```git add .```
  2. ```git commit -m "修改描述"```
  3. ```git push origin master```
