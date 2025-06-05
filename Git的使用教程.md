1. 创建版本库
	- step1：点击自己的文件目录，右键打开Git Bash
	- step2：`git init`  将当前目录变成可以管理的仓库
	- step3:   `git add` 将当前文件储存进暂存区
	- step4：`git commit` 将修改后的版本提交至仓库

2. 修改版本查看
	- step1：`git status` 检查是否有修改，显示modified表示有修改
	- step2：`git diff Git的使用教程.md` 可以显示具体修改的内容

3. 提交修改
	- step1:   `git add 文件名`
	- step2：`git status`  检查要提交的是否是修改过的文件
	- step3：`git commit` 提交修改过的文件版本
	- step4：`git status` 检查是否已经提交

4. Git的版本管理与回退
	- 版本管理：`git log` 可以查看历次的版本与对应的id
	- 版本回退：
		```
			 git reset --hard HEAD^  #回退到上个版本
			 git reset --hard HEAD^^  #回退到上上个版本
			 git reset --hard HEAD~100  #回退到100个版本以前
		```
	- 版本找回：`git reset --hard <commit id>`
	- 撤销修改
		1. 撤销工作区的修改：`git checkout -- 文件名`
		2. 撤销暂存区的修改：`git reset HEAD 文件名`

5. 文件的删除与回退
	- 工作区删除：`rm 文件名`
	- 暂存区删除：`git rm 文件名`  且 `git commit`
	- 暂存区盘面退回工作区：`git checkout -- 文件名`

6. 哈哈哈哈
