# iperf #
## 1.UDP灌包 ##
### 发送侧CMD ###
> iperf -u -c xx.xx.xx.xx -b 10m -i 1 -l 1000 -p 6003 -t 99999
### 接收侧CMD ###
> iperf -u -s -i 1 -p 6003
## 2.TCP灌包 ##
### 发送侧CMD ###
> iperf -c xx.xx.xx.xx -w 512k -p 6003 -t 9999999
### 接收侧CMD ###
> iperf -s -w 512k -p 6003
