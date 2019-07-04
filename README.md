世界上最难的事情就是习惯了Mac上的IDEA快捷键之后在Windows上用IDEA

# 如何使用
## 找到IDEA的Keymap配置文件
Windows and *NIX systems: `<User home>/.IntelliJ IDEA<xx>/config/keymaps` like `C:\Users\win\.IntelliJIdea2018.2\config\keymaps`  
macOS: `~/Library/Preferences/IntelliJ IDEA<xx>/keymaps`

## 把本项目的文件复制进去
把Mac OS X 10_5 on Windows.xml 放到 `keymaps` 文件夹里，没有文件夹就创建一个

## 重启IDEA
重启后【Setting】 -> 【Keymap】 选择 【Mac OS X 10_5 on Windows】

# !!!Important!!!
关掉类似QQ那些会占用你快捷键的软件

# 缺点
IDEA内的Alt用的很爽，但跟Windows的Ctrl键不协调

另一种方式是将本项目文件里的ctrl全部修改为alt，然后在Windows中全局互换Ctrl和Alt，可使用MapKeyboard

但Ctrl + Tab快捷键变成了Alt + Tab很不爽，可使用AutoHotkey将Windows的切换窗口快捷键修改为Alt + Tab：
1. 安装AutoHotkey
2. 创建一个新的文件：xxx.ahk，内容为`LCtrl & Tab:: AltTab`
3. 运行该文件
