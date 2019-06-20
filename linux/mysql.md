* 登录  
`mysql -uroot -p`
* 修改密码  
`update mysql.user set password=PASSWORD('root') where User='root';`
`flush privileges;`
* 查看编码
`SHOW VARIABLES WHERE Variable_name LIKE 'character%' OR Variable_name LIKE 'collation%';`
