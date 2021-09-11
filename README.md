## Configure Terminator

1.**Shortcuts*

+ `Ctrl+Shift+T`	新建一个terminator窗口
+ `Ctrl+Shift+E`	对terminator窗口垂直分割
+ `Ctrl+Shift+O`	对terminator窗口水平分割
+ `Ctrl+Shift+W`	关闭当前的terminator窗口
+ `Ctrl+Shift+I`	另外创建一个新的terminator窗口
+ `Ctrl+Shift+N`	在分割的不同窗口之间切换（向后）
+ `Ctrl+Shift+P`	在分割的不同窗口之间切换（向前）
+ `Ctrl+Shift+T`	新建一个Tab窗口
+ `Ctrl+Tab`	    切换下一个窗口
+ `Ctrl+Shift+T`	新建一个terminator窗口
+ `Ctrl+Shift+F`	当前terminator窗口进行搜索
+ `Ctrl+Shift+X`	当前分割的窗口最大化
+ `Alt+A`         将所有分割terminator同步
+ `Alt+O`	        关闭分割terminator同步




2.**install and uninstall** 

`sudo apt-get install terminator`  
`sudo apt-get remove terminator`

3.**configure file**

`gedit ~/.config/terminator/config`

```bash
[global_config]
  title_transmit_bg_color = "#d30102"
  focus = system
  suppress_multiple_term_dialog = True
[keybindings]
[profiles]
  [[default]]
    palette = "#2d2d2d:#f2777a:#99cc99:#ffcc66:#6699cc:#cc99cc:#66cccc:#d3d0c8:#747369:#f2777a:#99cc99:#ffcc66:#6699cc:#cc99cc:#66cccc:#f2f0ec"
    background_color = "#2D2D2D" # 背景颜色
    background_image = None   
    background_darkness = 1 
    cursor_color = "#2D2D2D" # 光标颜色
    cursor_blink = True # 光标是否闪烁
    foreground_color = "#EEE9E9" # 文字的颜色
    use_system_font = False # 是否启用系统字体
    font = Ubuntu Mono 13  # 字体设置，后面的数字表示字体大小
    copy_on_selection = True # 选择文本时同时将数据拷贝到剪切板中
    show_titlebar = False # 不显示标题栏，也就是 terminator 中那个默认的红色的标题栏
[layouts]
  [[default]]
    [[[child1]]]
      type = Terminal
      parent = window0
      profile = default
    [[[window0]]]
      type = Window
      parent = ""
[plugins]
```



