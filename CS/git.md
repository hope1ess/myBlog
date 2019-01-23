# 一些Git的使用技巧和心得
## Git版本回退
通过git log命令可以查看commit，显示出来的记录是降序的。
通过:
>git reset --hard HEAD^
可以回退到上一个版本，HEAD是一个指针，指向当前的版本。
## 工作区和暂存区的概念
>工作区就是在你电脑里可以看到的目录  

通过**git add**添加的文件，是把修改的内容添加到暂存区  
之后**git commit**，把暂存区的内容提交到分支上
## 撤销修改
>git checkout --test.txt

就是撤销test.txt在暂存区里的内容
## 删除文件
git rm + 已删除文件名，再commit一次就可以了。  
误删文件可以通过git checkout + 文件名，一键还原（此操作要在commit之前）
## 远程仓库
提交至远程仓库
>git push -U origin master
## 分支管理
