# git push -u origin master
> -u 设置上游分支（默认分支) 
> git push (默认推送到上游分支/默认分支)

# 团队开发实践

1. git init or git clone remote
 git remote add github git@github.com:outsider-persl/CS.git
2. git branch newbranch
- git branch dev
- git checkout dev 
- `coding and work`
- git push origin dev
3. git merge branche
- git checkout master
- git merge dev
