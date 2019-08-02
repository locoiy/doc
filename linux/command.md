* sudo chmod -R 777 目录名
```
备注：
  -R     是指级联应用到目录里的所有子目录和文件
  777    是所有用户都拥有最高权限（可自定权限码）
```
* ps -ef|grep tomcat|grep -v grep|awk '{print $2}'
```
备注：
  grep -v grep 过滤含有grep的行
  awk '{print $2}' 筛出第2域
```
* du -sh
```
  查看文件大小
```
