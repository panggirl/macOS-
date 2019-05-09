# Mac修改主机名和计算机名
* macOs 终端下的命令提示符是可以自定义的，通常命令提示符包含主机名(cui@xmf119)，也就是当前终端连接的主机的名称。
对于 Mac OS 下的终端来说，此时显示的“主机名”就是 HostName，也就是主机真正的名称，我们可以通过命令查看当前的“主机名”：
```
cui@xmf119  ~  hostname                             
xmf119
```
* Mac OS 下的“计算机名”，即 ComputerName 即是 ”系统偏好设置“——“共享”下的电脑名称,
这个名称也是同一局域网内其他用户看到的自己的计算机名称如macOS 的隔空投送下看到的名称

# 修改 在终端下，通过命令实现
```
sudo scutil --set HostName 新的主机名

sudo scutil --set ComputerName 新的计算机名
```
