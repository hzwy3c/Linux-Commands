### scp

配置ssh连接后，在`~/.ssh/config`文件中加入

```
Host myserver
    HostName IP地址或域名
    User 用户名
```

`myserver`即是服务器别名，可以直接用

1. `scp source destination`：将`source`路径下的文件复制到`destination`中国
2. `scp source1 source2 destination`：一次复制多个文件
3. `scp -r  ~/tmp myserver:/home`：将本地家目录中的`tmp`文件夹复制到`myserver`服务器中的家目录下
4. `scp -P 22 source1 source2 destination`：指定服务器的端口号
5. `scp ~/.vimrc ~/.tmux.conf myserver:`：使用`scp`配置其他服务器的`vim`和`tmux`