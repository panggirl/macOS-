# zsh: command not found: adb

安装完zsh，在使用相关shell命令，出现了”zsh: command not found adb:adb”,”zsh: command not found: git” 等一系列error

其实就是bash shell 以及zsh shell 是两种读取系统环境变量 
（使用adb的前提是你肯定已经在bash的 .bash_profile 已经配置相关android tool的环境变量了，从而才能使用adb命令）

然而在使用zsh shell的时候，你并没有把相关的环境变量的配置设置到 .zshrc 中（功能上类似bash 的.bash_profile）

解决办法:既然是.zshrc 没有配置相关环境变量设置，把 bash 中.bash_profile 全部环境变量加入就好
```
open .zshrc
```
然后找到# User configuration部分，添加
```
# User configuration
source ~/.bash_profile
```
