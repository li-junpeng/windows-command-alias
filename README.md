# windows-command-alias
command alias in windows powershell

# How use?
1. 打开powershell
2. 在命令窗口中输入`echo $PROFILE`查看一下配置文件的路径.
3. 打开配置文件就可以自定义咱们的命令别名啦~

# My command alias
```shell
function ll {dir $args}
function mv {Rename-Item $args}
function cp {Copy-Item $args}
function rm {Remove-Item $args}

function port {netstat -ano | findstr $args}

# git
function g-s {git status $args}
function g-a {git add $args}
function g-c {git commit -m $args}
function g-p {git push $args}
function g-pl {git pull $args}
function g-check {git cherry -v $args}

#node 
function nd {npm run dev}

# dir path
function codestore {cd 'D:\0 Code Store'}
function dbtu {cd 'D:\0 Code Store\dbtu'}
```
