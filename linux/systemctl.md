# systemctl 命令有两大类功能：  
  * 控制 systemd 系统  
  * 管理系统上运行的服务
# Commands
  >* systemctl --version    *查看版本号*
  >* whereis systemctl    *查看systemctl程序的相关目录
## systemctl [command] [unit]
  >* start：立刻启动后面接的 unit。
  >* stop：立刻关闭后面接的 unit。
  >* restart：立刻关闭后启动后面接的 unit，亦即执行 stop 再 start 的意思。
  >* reload：不关闭 unit 的情况下，重新载入配置文件，让设置生效。
  >* enable：设置下次开机时，后面接的 unit 会被启动。
  >* disable：设置下次开机时，后面接的 unit 不会被启动。
  >* status：目前后面接的这个 unit 的状态，会列出有没有正在执行、开机时是否启动等信息。
  >* is-active：目前有没有正在运行中。
  >* is-enable：开机时有没有默认要启用这个 unit。
  >* kill ：不要被 kill 这个名字吓着了，它其实是向运行 unit 的进程发送信号。
  >* show：列出 unit 的配置。
  >* mask：注销 unit，注销后你就无法启动这个 unit 了。
  >* unmask：取消对 unit 的注销。
## systemctl [command] [--type=TYPE] [--all]    *查看系统上的unit*  
  >* list-units：列出当前已经启动的 unit，如果添加 -all 选项会同时列出没有启动的 unit。
  >* list-unit-files：根据 /lib/systemd/system/ 目录内的文件列出所有的 unit。
  >* --type=TYPE：可以过滤某个类型的 unit。
  >* 不带任何参数执行 systemctl 命令会列出所有已启动的 unit
  ` 比如只想查看服务类的unit：systemctl list-units --type=service --all `
