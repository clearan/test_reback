## 版本回退
### 没有push到远程分支
```text
1、git reset --soft + 版本号 ------->只撤销commit
2、git reset --mixed + 版本号 ------->撤销add和commit
```
###已经push到远程分支
```text
1、git reset --hard + 想要回退到的版本号  --->会将回退到目标版本之后的提交记录清空，不推荐使用。并且需要强制push,git push -f
2、git revert 当前的版本号。撤销当前的提交，保留记录。 
3、git revert -n + 版本号  撤销某次提交，不影响别的提交
```
