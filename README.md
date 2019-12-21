# How To Use Git Branch
1. 分支的创建
* 第一种方法
```
git branch Test
// 创建一个名为Test的分支
```
- 第二种方法
```
git checkout -b Test
// 创建一个名为Test的分支并立即切换到该分支
```
> 显示所有分支  
> git branch -a
2. 分支的切换
```
git checkout Test
// 切换到Test分支
```
> **注意：**
>> 如果不在master分支需要在当前分支下进行commit操作，不然删除文件master的文件也会被删除

3. 分支的推送
```
git push --set-upstream origin Test
// 在远程建立一个名为Test的分支并与本地分支关联
```
> 其他操作方法一样
4. 分支的删除
- 本地分支删除
```
git branch -d Test
// 删除一个名为Test的本地分支
```
- 远程分支删除
```
git push origin --delete Test
// 删除一个名为Test的远程分支
```