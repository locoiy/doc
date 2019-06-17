* 登录  
`mysql -uroot -p`
* 修改密码  
```
  update mysql.user set password=PASSWORD('root') where User='root';
  flush privileges;
```
