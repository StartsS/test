##### 初始本地化库
- `git init`

#####  设置签名
用途为了标识身份，通常只设置全局级别
- 设置仓库级别签名：
`git config user.name jsm`
`git config user.email jsmxok@163.com`
- 设置全局级别签名：
`git config --global user.name jsm`
`git config --global user.email jsmxok@163.com`

#####  分支操作
- 创建分支
git branch [分支名]
-  查看分支
git branch -v
- 切换分支
git checkout [分支名]
- 合并分支
 第一步：切换到接受修改的分支（被合并，增加新内容）上 

		git checkout [被合并分支名]
	第二步：执行 merge 命令

			git merge [有新内容分支名]
- 解决冲突
  1. 冲突的表现
![在这里插入图片描述](https://img-blog.csdnimg.cn/2019052409093411.png?x-oss-process=image/watermark,type_ZmFuZ3poZW5naGVpdGk,shadow_10,text_aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L2pzbW9rX3hpbmdrb25n,size_16,color_FFFFFF,t_70)
  2. 冲突的解决
	第一步：编辑文件，删除特殊符号
	第二步：把文件修改到满意的程度，保存退出
	第三步：git add [文件名]
	第四步：git commit -m "日志信息"  （ 注意：此时 commit 一定不能带具体文件名）
