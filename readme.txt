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
克隆 git clone +地址	（git支持多种协议）
创建分支 git checkout -b 分支名 (-b表示创建并切换) 创建分支 git branch <name>切换分支 git checkout <name>
查看当前分支 git branch
分支合并 git merge <name>
删除分支 git branch -d <name>
分支合并冲突时需要手动解决冲突再提交，此时合并完成
查看分支合并图 git log --graph (--pretty=oneline 简要信息)
不以ff方式合并分支 git merge --no-ff -m "merge with no-ff" dev (会创建一个新的备注为""的commit)
中断机制 git stash 保存工作区状态，再查看是工作区为空
查看中断点 git stash list
恢复 git stash apply（不会删除stash） 删除 git stash drop
恢复并删除断点 git stash pop
多个断点： ~ stash@{*}
删除一个未合并的分支 git branch -D <name>（大写D）
