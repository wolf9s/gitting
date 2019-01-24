### delete git tag on gerrit
#### first: *create tag & push*
```
git tag -a v1.0.1

git push origin v1.0.1
```

#### second: *delete remote tag*

```
git tag -d v1.0.1

git push origin :refs/tags/v1.0.1
```

  > 注：需要设置相应的权限才能进行操作： 
gerrit 上相应的项目权限设置如下   
Reference: refs/tags/*  
[**Push**] 权限 +Force Push   
[**Push Annotated Tag**] 权限 +Force Push   
