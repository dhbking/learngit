1.git is a version control soft
2.git is a free soft

命令集：git config --global user.name "your name"
		git config --global user.email "email@example.com"
		git add <file>      					添加文件
		git commit -m "提交文件信息说明"
		git status          					获取版本库状态
		git diff <file>							获取文件所做的修改
		git log									查看提交历史
		git log --pretty=oneline				查看提交历史简约显示
		git reflog 								查看命令历史，可用于回到未来某版本
		git reset --hard HEAD^					回到上一版本
		git reset --hard <commit_id>			回到任意版本id
		git checkout -- <file>					当修改了工作区某个文件的内容，还未添加到暂存区时，想直接丢弃工作区的修改
		git reset HEAD <file>					当修改了工作区某个文件的内容，还添加到了暂存区时，使用该指令将取消添加修改到暂存区
		若已经提交了不合适的修改到版本库时，想要撤销本次提交，可进行版本回退，不过前提是没有推送到远程库
		rm <file>								从工作区中删除该文件
		可使用git checkout -- <file>把误删的文件恢复到最新版本，前提版本库中该文件未删除
		git rm <file>							从版本库中删除该文件，接着git commit即可完成删除
		