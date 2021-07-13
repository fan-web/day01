##场景一（较为繁琐，建本地仓库，获取连接什么的）
```
进入到桌面：cd Desktop  (返回上一级为 cd )
创建一个文件：mkdir test（文件名）
进入文件：cd test
把该文件建立成本地仓库：git init
添加文件:touch README.md（文件名）（此时工作区内有该文件，但未到本地仓库）
往本地仓库内添加文件：git add README.md（文件名）    git commit -m "add README.md file"（""里面相当于一个注释，尽量清晰明了）
查询本地仓库内文件:ls -la
本地仓库与远程仓库建立连接（远程仓库需要在github里面先建好，有url）：git remote add origin url
查询连接:git remote -v
上传文件:git push -u origin master（第一次用写"-u origin master"，往后不用）
注：在操作期间可以不断通过 git status 查看暂存区和本地仓库内文件的状态，用 git log 查看本地仓库的日志信息
```
##场景二（较为简便，从远程仓库提取过来的文件夹直接是本地仓库同时也已经自动创建好与远程仓库的连接）
```
进入桌面目录：cd Desktop
通过远程仓库的url进行克隆：git clone https://github.com/fan-web/day01.git(url（克隆远程仓库内的文件，同时在桌面上新建一个文件夹，为远程仓库内项目的名称）)
进入克隆过来的文件夹：cd day01(文件名字)
验证是否是本地仓库并存在文件：ls -la
可以新增文件(在day01文件目录下)：touch README.md   git add README.md   git commit -m "add README.md file"
查询进程及状态：git status    git log
上传文件：git push（有一定限制，别人的远程仓库个人是不能上传文件的）


注：使用git的时候，为了避免冲突，一定要先pull（更新），再push（上传）
```

