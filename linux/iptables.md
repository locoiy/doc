* 查看  
`iptables -nvL`
* 关闭所有的 INPUT FORWARD OUTPUT 只对某些端口开放
```
iptables -P INPUT DROP
iptables -P FORWARD DROP
iptables -P OUTPUT DROP
```
* 保存
`service iptables save`
* 看到信息 firewall rules 防火墙的规则 其实就是保存在 /etc/sysconfig/iptables
* 删除
` 通过 iptables -L -n --line-number 可以显示规则和相对应的编号 `
` iptables -D INPUT 2 `
