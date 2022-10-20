### tmux

功能：

- 分屏
- 允许断开Terminal连接后，继续运行进程

结构：

一个`tmux`可以包含多个`session`，一个`session`可以包含多个`window`，一个`window`可以包含多个`pane`

操作：

1. `tmux`：新建一个`session`，其中包含一个`window`，`window`中包含一个`pane`，`pane`里打开了一个`shell`对话框
2. 按下`Ctrl + a`后松开手指，然后按`%`：将当前`pane`左右平分成两个`pane`
3. 按下`Ctrl + a`后松开手指，然后按`"`：将当前`pane`上下平分成两个`pane`
4. `Ctrl + d`：关闭当前`pane`；如果当前`window`的所有`pane`均已关闭，则自动关闭`window`；如果当前`session`的所有`window`均已关闭，则自动关闭`session`
5. 按下`Ctrl + a`后松开手指，然后按方向键：选择相邻的`pane`
6. 按下`Ctrl + a`的同时按方向键，可以调整`pane`之间分割线的位置
7. 按下`Ctrl + a`后松开手指，然后按`z`：将当前`pane`全屏/取消全屏
8. 按下`Ctrl + a`后松开手指，然后按d：挂起当前`session`
9. `tmux a`或`tmux attach`：打开之前挂起的`session`
10. 按下`Ctrl + a`后松开手指，然后按`s`：选择其他`session`
    - 方向键↑：选择上一项`session/window/pane`
    - 方向键↓：选择下一项`session/window/pane`
    - 方向键←：展开当前项`session/window`
    - 方向键→：闭合当前项`session/window`
11. 按下`Ctrl + a`后松开手指，然后按`c`：在当前`session`中创建一个新的window
12. 按下`Ctrl + a`后松开手指，然后按`w`：选择其他`window`
13. 在`tmux`中选中文本时，需按住`shift`键（不支持`Mac`）
14. `tmux`中复制/粘贴文本的通用方式：
    - 按下`Ctrl + a`后松开手指，然后按`[`
    - 用鼠标选中文本，按下`Ctrl + a`后松开手指，然后按`]`，会将内容粘贴到光标处