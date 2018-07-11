添加到暂存区 git add<文件名>
提交 git commit -m '注释'
查看版本历史 git log，git log --pretty=oneline
替换版本 git reset --hard HEAD^^^,git reset --hard 版本号
查看历史历史命令 git reflog
查看文件状态 git status
对比工作区与版本库文件区别 git diff HEAD(可以是任意版本) -- <文件名>
用版本库中的内容替换工作区的内容 git checkout -- <file>
把暂存区的内容撤回工作区 git reset HEAD <file>
删除本地 rm 删除版本库中的文件 git rm
本地库推到远程 git push eg:git push -u origin master (-u 推送并关联)
