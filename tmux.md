### tmux

功能：

- 分屏
- 允许断开Terminal连接后，继续运行进程

结构：

一个`tmux`可以包含多个`session`，一个`session`可以包含多个`window`，一个`window`可以包含多个`pane`

操作：

1. `tmux`：新建一个`session`，其中包含一个`window`，`window`中包含一个`pane`，`pane`里打开了一个`shell`对话框

2. `tmux ls`：查看已经存在`session`

3. `tmux new -s name`：新建一个名为`name`的`session`

4. `tmux a -t name`：重新连接名为`name`的`session`，查看结果

5. `Ctrl + d`：关闭当前`pane`；如果当前`window`的所有`pane`均已关闭，则自动关闭`window`；如果当前`session`的所有`window`均已关闭，则自动关闭`session`

6. `Ctrl + b d`：先按`Ctrl+b`之后再按`d`，暂时退出session

   