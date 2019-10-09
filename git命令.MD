maven打包：

```
mvn -Dmaven.test.skip=true -Pdev -e clean package
```

# git命令

## 生成ssh rsa

```
ssh-keygen -t rsa -C "邮箱"
```


## 验证ssh是否配置成功

```
ssh -T git@github.com
```

成功显示如下

```
Hi SilverHu! You've successfully authenticated, but GitHub does not provide shell access.
```

## 添加项目到git

```
	git init
	git remote add origin git@github.com:yourName/yourRepo.git

	# 查看远程仓库
	git remote -vv
```

## 查看分支

```
# 查看所有分支
git branch -a

# 查看当前分支及对应远程分支
git branch -vv
```

## 强制检出/切换分支或分支指定文件

```
git checkout <branch> [file] [-f]
```

## 添加文件加入git版本库中

```
# 添加所有文件
git add -A

# 添加单个文件
git add 文件名
```

## 删除git版本库中文件

```
git rm 文件名
git rm -r 文件夹名
```

## 提交到本地仓库

```
git commit -m "描述信息"
```

## 查看已合并|未合并的本地仓库分支

```
git branch [--merged | --no-merged]
```

## 分支合并

```
git merge <branch name>
```

## 删除远程分支

```
git push origin :branch-name
```

## 推送本地仓库代码到远程仓库

```
git push [remote_branch] [local_branch]
```

## 取消暂存

```
git reset [file]
```

## 恢复文件

```
git checkout -- [file]
```

## 新建分支並立即切換到新分支

```
git checkout -b <branch_name> <origin_name>

# 修改分支名称
git branch -m <new_name> 
```

	
