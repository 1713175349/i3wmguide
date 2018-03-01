目录
[1.默认快捷键](#1)
[2.使用i3](#2)
[2.1.打开终端并且移动它](#2.1)
[2.2改变容器布局](#2.2)
<h2 id="1">1.默认快捷键</h2>
对于那些不喜欢看长文字的人，这是一个默认快捷键总览
只使用$mod键的快捷键：
＞![](https://i3wm.org/docs/keyboard-layer1.png)
使用Shift+$Mod的快捷键：
![](https://i3wm.org/docs/keyboard-layer2.png)
在执行蓝色键所表明操作时，红色键都得按住
值得注意的是，当你没有配置文件打开i3时，i3-config-wizard将让你选择bkey键上图中的键，不管你的键盘布局是什么．如果你更喜欢上图所示的快捷键，只需要拒绝i3-config-wizard默认以/etc/i3/config为配置文件
<h2 id="2">2.使用i3</h2>
本手册中，$mod将被习惯的用于配置文件．Alt键（Mod1)是默认键，Win键是另一个流行的选择
<h3 id="2.1">2.1.打开终端并且移动它</h3>
打开新的终端是一种常规操作．默认快捷键是$mod+Enter，默认配置是Alt+Enter.按住$mod+Enter,一个新的终端就打开了．它将充满屏幕上的可用空间
![](https://i3wm.org/docs/single_terminal.png)
如果你打开一个新的终端，i3会把它放置在已有终端下面，它们平分整otherw目录
[1.默认快捷键](#1)
[2.使用i3](#2)
[2.1.打开终端并且移动它](#2.1)
[2.2改变容器布局](#2.2)
<h2 id="1">1.默认快捷键</h2>
对于那些不喜欢看长文字的人，这是一个默认快捷键总览
只使用$mod键的快捷键：
＞![](https://i3wm.org/docs/keyboard-layer1.png)
使用Shift+$Mod的快捷键：
![](https://i3wm.org/docs/keyboard-layer2.png)
在执行蓝色键所表明操作时，红色键都得按住
值得注意的是，当你没有配置文件打开i3时，i3-config-wizard将让你选择bkey键上图中的键，不管你的键盘布局是什么．如果你更喜欢上图所示的快捷键，只需要拒绝i3-config-wizard默认以/etc/i3/config为配置文件
<h2 id="2">2.使用i3</h2>
本手册中，$mod将被习惯的用于配置文件．Alt键（Mod1)是默认键，Win键是另一个流行的选择
<h3 id="2.1">2.1.打开终端并且移动它</h3>
打开新的终端是一种常规操作．默认快捷键是$mod+Enter，默认配置是Alt+Enter.按住$mod+Enter,一个新的终端就打开了．它将充满屏幕上的可用空间
![](https://i3wm.org/docs/single_terminal.png)
如果你打开一个新的终端，i3会把它放置在已有终端下面，它们平分整otherwise个屏幕．依靠你的配置，i3将将新建的窗口放置在已有窗口的旁边或下面．
![](https://i3wm.org/docs/two_terminals.png)
将焦点在两个终端间移动，你能使用方向键，像使用vim/vi一样．然而，在i3里，你的homerow键（指打字时手指所放的准备位置）也被用于这些键．因此，$mod+j是左，$mod+k是下,$mod+l是上,$mod+;是右．所以，使用$mod+k或者$mod+l在两个终端间切换．当然也能用方向键．
现在你的工作空间在一个特殊的方向上分成两份（默认水平分）．每个窗口也能在一次被水平分或者垂直分，像工作空间一样．
垂直分割：$mod+v
水平分割：$mod+h
<h3 id="2.2">2.2.改变容器布局</h3>
一个分离容器能有以下任意一种布局：
splith/splitv

> 窗口是有大小的，因此每个窗口在容器中有相同的空间．splith水平分割（窗口左右分布），splitv垂直分割（窗口上下分布）
> stacking(堆叠)
> 只有目前聚焦的窗口在容器中显示．在容器上方显示窗口列表．
> tabbed
> 原理和stacking相同，但窗口列表只是顶部的一条线
> ![](https://i3wm.org/docs/modes.png)
> 选择模式：
> splith/splitv:$mod+e
> stacking:$mod+s
> tabbed:$mod+w
> <h3 id="2.3">2.3.切换窗口是否全屏</h3>
> 使窗口全屏或者使全屏窗口恢复，按$mod+f.
> i3也有一个全局全屏模式，在这个模式客户端将跨越所有输出（命令是fullscreen toggle global)
> <h3 id="2.4">2.4.打开其他软件</h3>
> 除了从终端打开程序，你也可以使用方便的dmenu，默认用$mod+d打开dmenu．只要输入想要打开程序名称或一部分．相应的程序必须在PATH变量里．此外，如果你有些程序用得很频繁，你可以创建一个快捷键．详见[配置文件](#4)
> <h3 id="2.5">关闭窗口</h3>
> 如果程序没有提供一个关闭方式（大多数程序提供一个菜单，退出键或者ctrl+w快捷键来关闭），你可以用$mod+Shift+q来杀死一个窗口．对于提供WM_DELETE协议的程序，这将合理的关闭程序（存储任何修改，清除垃圾）．如果没有提供这个协议，你的X服务器将杀死窗口，这个行为依靠这个程序．
> <h3 id="2.6">使用工作空间</h3>
> 工作空间是一种把窗口组织起来的简单方式．默认是在第一个工作区间，它在底部状态栏左侧显示．切换到另一个工作区，按$mod+想切换到工作区的数字．如果它不存在，就会创建．
> 如果你有多个屏幕，一个工作区将在开启时在每个屏幕上创建．如果你打开一个新的工作区，它将跳到你创建时的屏幕．当你切换到另一个屏幕上的工作区，i3将聚焦到那个屏幕
> <h3 id="2.7">移动窗口到其他工作区</h3>
> 只要按$mod+Shift+num将窗口移动到目标工作区．同样如果工作区不存在也会创建．
> <h3 id="2.8">改变大小</h3>
> 最简单的方法是用鼠标：拖边界到想到大小
> 你也能用[捆绑模式](#4.5)去定义一个模式通过键盘改变大小．看一个简单的例子：看i3的[默认配置](https://github.com/i3/i3/blob/next/etc/config.keycodes)
> <h3 id="2.9">重启i3</h3>
> 重启i3可以使用$mod+Shift+r
> <h3 id="2.10">退出i3</h3>
> 干净的关闭i3而不杀死X服务器，你可以使用$mod+Shift+e.默认会弹出提示框让你确认．
> <h3 id="2.11">悬浮模式</h3>
> 悬浮模式和平铺模式相反．窗口的位置和大小不是被i3自动管理，而是由你手动管理．使用这个模式违反平铺，但对于一些小情形如＂保存为＂对话框，或者工具栏很有用．这种窗口通常设置适当的提示并默认以悬浮模式打开．
> 你能使用$mod+Shift+Space将一个窗口切换到悬浮模式．通过鼠标用鼠标拖标题栏能四处移动窗口．拖动边缘能改变大小．也能通过[浮动修改器](#.4.6)做到这些．
> <h2 id="3">树</h2>
> i3将所有关于X11输出、工作区和窗口布局的信息存储在树中.根节点是X11根窗口，紧接着是X11输出，然后是码头区域和一个内容集装箱，再然后工作区和窗口自己．在之前的i3版本中，我们有多个列表(输出、工作区)和每个工作区的表．这种方法被证明是复杂，难用，难以理解．
> <h3 id="3.1">由容器组成的树</h3>
> 树的构件叫做容器．容器能承载一个窗口（一个X11窗口）．另外，它包含一个或多个容器．一个简单的例子是工作区：但你在单屏幕打开i3，在一个工作区打开两个终端，最终你会得到一个这样的树：
> ![](https://i3wm.org/docs/tree-layout2.png)
> <h3 id="3.2">定位和分离容器</h3>
> 在使用树作为数据结构时，使用所谓的分割容器是很自然的事情。每个容器都有一个定位(水平、垂直或未指明的方向)，而方向取决于容器的布局(垂直：splitv,stacking,水平:splith,tabbed).因此，在我们的工作空间示例中，工作区容器的默认布局是splith(现在大多数显示器都是宽屏).如果你把布局改变为splitv,然后打开两个终端，i3将配置你的桌面如下：
> ![](https://i3wm.org/docs/tree-shot2.png)
> i3自版本４以来有一个有趣的新特性，就是能够分开任何东西：假使你有在同一个工作区两个终端（使用splith布局，水平定位），聚焦在右侧终端．现在如果你要打开另一个终端在现在这个终端的下面．如果你仅仅只是打开新的终端，由于splith布局的作用，新终端会在右侧．因此你需要按$mod+v切换布局到垂直模式．现在你就能在当前终端下方打开终端了．
> ![](https://i3wm.org/docs/tree-shot1.png)
> ![](https://i3wm.org/docs/tree-layout1.png)
> 你也许早就猜到了：分裂等级的深度是没有限制的
> <h3 id="3.3">聚焦到父级节点</h3>
> 保持上一节的例子．左边有一个终端右边有两个垂直的分屏终端，焦点在右下方．当你打开一个新的终端时，它会在当前的这个终端下方打开．所以怎样在当前终端右侧打开呢？解决方案是使用focus parent(默认是$mod+a)这将聚焦到当前容器的父级容器．如果这样，您将聚焦到垂直分割容器，位于水平方向的工作区中．因此，现在新的窗口将在垂直分割的容器的右侧．
> ps:值得注意的是，垂直分割的容器的布局是splith
> <h3 id="3.4">隐式容器</h3>
> 在某些情况下，i3需要隐式地创建一个容器来实现您的命令。一个示例是这样的场景：您使用一个单独的显示器器启动i3，以及在其中打开三个终端窗口的单个工作区。所有这些终端窗口都直接连接到i3的布局树中的一个节点，即工作区节点。默认情况下，工作区节点的方向是水平的。
> 现在你向下移动其中一个终端（默认是$mod+Shift+k）．工作空间节点的方向将被更改为垂直．您移动的终端窗口直接连接到工作区，并出现在屏幕的底部。创建了一个新的(水平的)容器，以容纳另外两个终端窗口。当切换到选项卡模式时，您就会注意到这一点.最后，您将得到一个带有拆分容器(例如“H[urxvt firefox]”)的标签，而另一个选项卡则是您移动的终端窗口。
> <h2 id="4">配置i3</h2>
> 这才是真正有趣的开始;-）。大多数东西都非常依赖于你理想的工作环境，所以我们不能为它们做出合理的默认设置.
> 尽管没有用编程语言,i3对于一般窗口管理器所做的事也相当灵活.
> 例如，您可以配置绑定快捷键来跳转到特定的窗口，您可以设置特定的应用程序以启动特定的工作空间，您可以自动启动应用程序，您可以更改i3的颜色，您可以绑定您的键来做有用的事情。
> 改变i3的配置,复制/etc/i3/config到~/.i3/config(或者~/.config/i3/config,如果你喜欢XDG目录计划),并且用编辑器编辑它.
> 第一次启动时(除非你已经有一个配置文件了),i3将提议你去创建一个配置文件.你可以告诉向导程序在配置文件中使用Alt(Mod1)或者Win(Mod4)作为mod键.同样,新建的配置文件将使用你目前的键盘布局.使用命令 i3-config-wizard打开向导程序.请确认你没有~/.i3/config文件,否则将退出引导程序.
> 自i3 4.0以来,使用了一种新的配置文件格式.3将尝试基于几个不同的关键字自动检测配置文件的格式版本，但是如果你想确保你的配置是用新的格式读取的，那么在你的配置文件中包括以下一行:

```
# i3 config file (v4)
```

<h3 id="4.1">注释</h3>
可以在您的配置文件中使用注释来正确地记录您的设置，以便以后引用.注释是用#开头的，也只能在一行的开头使用:
例子:

```
# This is a comment
```

<h3 id="4.2">字体</h3>
i3支持X核心字体和自由字体（通过Pango）来渲染窗口标题.要生成X核心字体描述，您可以使用xfontsel(1).要查看特殊字符(Unicode)，需要使用支持iso-10646编码的字体.自由字体描述由字体家族、样式、重量、变体、拉伸和大小组成。FreeType字体支持从右到左的渲染，并且包含比X核心字体更多的Unicode字符.如果i3不能打开配置好的字体，它会在日志文件中输出一个错误，然后返回一个工作的字体.
语法:

```
font <X core font description>
font pango:<family list> [<style options>] <size>
```

例子:

```
font -misc-fixed-medium-r-normal--13-120-75-75-C-70-iso10646-1
font pango:DejaVu Sans Mono 10
font pango:DejaVu Sans Mono, Terminus Bold Semi-Condensed 11
font pango:Terminus 11px
```

<h3 id="4.3">按键绑定</h3>
键盘绑定使i3在按下特定键时执行命令(见下)。i3允许你在键码或键符号上绑定(你也可以混合你的绑定，不过i3不会保证你不重叠的).
+键符是一个特定的符号描述,像"a","b",但也有更奇怪的,像用"underscore"而不是"_".这是你在xmodemap中用来重新映射按键的符号.使用xmodmap -pke得到目前的键盘映射.要交互式地输入一个键并查看它被配置为什么键可以使用xev.
+键码不需要指定一个符号,当你切换到不同的键盘布局时(使用xmodmap)，它们不会改变它们的意思.
我的建议是:如果你经常切换键盘布局，但你想把你的绑定放在键盘上相同的物理位置上，使用键盘代码.如果您不切换布局，并且想要一个简洁且简单的配置文件，请使用键符.
有些工具(如import,xdotool)也许不能在按键事件上运行,因为键盘/鼠标指针仍然被占据.对于这种情形,可以使用--release标志,这将使命令在键被释放后执行.
语法:

```
bindsym [--release] [<Group>+][<Modifiers>+]<keysym> command
bindcode [--release] [<Group>+][<Modifiers>+]<keycode> command
```

例子:

```
# Fullscreen
bindsym $mod+f fullscreen toggle

# Restart
bindsym $mod+Shift+r restart

# Notebook-specific hotkeys
bindcode 214 exec --no-startup-id /home/michael/toggle_beamer.sh

# Simulate ctrl+v upon pressing $mod+x
bindsym --release $mod+x exec --no-startup-id xdotool key --clearmodifiers ctrl+v

# Take a screenshot upon pressing $mod+x (select an area)
bindsym --release $mod+x exec --no-startup-id import /tmp/latest-screenshot.png
```

可用修饰符:
Mod1-Mod5, Shift, Control ,Standard modifiers, 看 xmodmap(1)
Group1, Group2, Group3, Group4 
当你使用多个键盘布局(e.g. :  setxkbmap -layout us,ru),你可以指定哪个XKB组(或称布局)将被激活.默认按键绑定在Group1,并在所有组激活.如果你想在你的一个布局中重写键绑定,指定对应的组即可.对于向后兼容，组“Mode_switch”是Group2的别名.
<h3 id="4.4">鼠标绑定</h3>
鼠标绑定，在单击了的容器的范围内按下特定的鼠标按钮后使i3执行一个命令.您可以以类似于键绑定的方式配置鼠标绑定。
语法:

```
bindsym [--release] [--border] [--whole-window] [--exclude-titlebar] [<Modifiers>+]button<n> command
```

默认情况下，绑定只在单击窗口的标题栏时才会运行.如果给定了--release标志它将在鼠标按钮被释放时运行.
如果给定了 --whole-window标志,当窗口的任何部分除了边界之外被单击时，绑定也会运行.指定--border标志,在边界被点击时运行.
如果给定了--execlude-titlebar标签,标题栏不会包括进去.
例子:

```
# The middle button over a titlebar kills the window
bindsym --release button2 kill

# The middle button and a modifer over any part of the window kills the window
bindsym --whole-window $mod+button2 kill

# The right button toggles floating
bindsym button3 floating toggle
bindsym $mod+button3 floating toggle

# The side buttons move the window around
bindsym button9 move left
bindsym button8 move right
```

<h3 id="4.5">模式绑定</h3>
通过使用不同的绑定模式，您可以拥有多个绑定集.当您切换到另一个绑定模式时，当前模式下的所有绑定都将被释放，只有在新模式下定义的绑定才有效，只要您保持在这种绑定模式下.唯一的预定义绑定模式是默认模式，即i3开始时使用的模式，以及在特定绑定模式下没有定义的所有绑定.
绑定模式的工作由两部分组成:定义绑定模式并切换到绑定模式。出于这些目的，有一个配置指令和一个命令，这两个命令都被称为模式。该指令用于定义属于某个绑定模式的绑定，而命令用于切换到指定模式.
推荐使用[变量](#4.14)使维护更加容易.下面是一个如何使用模式绑定的例子.
注意:定义一个返回默认模式的绑定是明智的.
注意:可以使用[pango_markup]进行模式绑定,但必须模式定义时传入--pango_markup标记.
语法:

```
# config directive
mode [--pango_markup] <name>

# command
mode <name>
```

例子:

```
# Press $mod+o followed by either f, t, Escape or Return to launch firefox,
# thunderbird or return to the default mode, respectively.
set $mode_launcher Launch: [f]irefox [t]hunderbird
bindsym $mod+o mode "$mode_launcher"

mode "$mode_launcher" {
    bindsym f exec firefox
    bindsym t exec thunderbird

    bindsym Escape mode "default"
    bindsym Return mode "default"
}
```

<h3 id="4.6">悬浮修饰符</h3>
要用鼠标移动浮动窗口，你可以抓取它们的标题栏,或者配置所谓的浮动修饰符你可以点击并点击窗口的任何地方来移动它.最常见的设置是使用与管理windows相同的密钥（例如Mod1).然后你可以按下Mod1，用鼠标左键点击一个窗口，然后拖拽到你想要的位置.当你持有浮动的修改器时，你可以通过按下鼠标右键并再按住的同时移动来调整浮动窗口的大小.如果你按住shift键，那么调整的大小将是成比例的(相位比例将被保留).
语法:

```
floating_modifier <Modifier>
```

例子:

```
floating_modifier Mod1
```

<h3 id="4.7">限制悬浮窗口大小</h3>
可以指定浮动窗口的最大和最小尺寸.如果指定floating_maximum_size其中一个唯独指定为-1,这个维度将将没有最大值的限制.如果没有定义floating_maximum_size,或者指定为0,i3将使用默认的值限制窗口的最大值.floating_minimum_size也类似.
语法:

```
floating_minimum_size <width> x <height>
floating_maximum_size <width> x <height>
```

例子:

```
floating_minimum_size 75 x 50
floating_maximum_size -1 x -1
```

<h3 id="4.8">为新窗口定模式</h3>
新的工作空间得到合理的默认方向:宽屏显示器(宽大于高)得到水平方向,旋转了的屏幕(高大于宽)得到垂直方向.使用default_orientation配置指令，您可以覆盖该行为.
语法:

```
default_orientation horizontal|vertical|auto
```

例子:

```
default_orientation vertical
```

<h3 id="4.9">新容器的布局模式</h3>
该选项确定工作空间级别的新容器将在哪个模式下启动。
语法:

```
workspace_layout default|stacking|tabbed
```

例子:

```
workspace_layout tabbed
```

<h3 id="4,10">新窗口的边框样式</h3>
这个选项决定了新窗口的边界样式.默认值是normal.请注意，新的浮动只适用于windows，它是作为浮动窗口开始的，例如，对话框窗口，而不是稍后浮动的窗口.
语法:

```
new_window normal|none|pixel
new_window normal|pixel <px>
new_float normal|none|pixel
new_float normal|pixel <px>
```

例子:

```
new_window pixel
```

“正常”和“像素”边界样式支持一个可选的边框宽度:
例子:

```
# The same as new_window none
new_window pixel 0

# A 3 px border
new_window pixel 3
```

<h3 id="4.11">隐藏与屏幕边缘相邻的边框</h3>
您可以使用hide_edge_borders来隐藏与屏幕边缘相邻的容器边界.如果您使用滚动条，或者不想在显示空间中浪费两个像素，那么这非常有用."smart"设置在工作区只有一个窗口可见时隐藏边框,但在同一工作区多个窗口可见时不隐藏.默认是"none".
语法:

```
hide_edge_borders none|vertical|horizontal|both|smart
```

例子:

```
hide_edge_borders vertical
```

<h3 id="4.12">对于特定窗口的任意命令(for_window)</h3>
对于for_window命令,能让i3执行任何命令当它遇到指定窗口时.这可以用来设置窗口浮动或改变边框样式.
语法:

```
for_window <criteria> <command>
```

例子:

```
# enable floating mode for all XTerm windows
for_window [class="XTerm"] floating enable

# Make all urxvts use a 1-pixel border:
for_window [class="urxvt"] border pixel 1

# A less useful, but rather funny example:
# makes the window floating as soon as I change
# directory to ~/work
for_window [title="x200: ~/work"] floating enable
```

有效的标准与命令的标准是相同的
<h3 id="4.13">不聚焦到打开的窗口</h3>
no_focus命令能阻止一个新打开的窗口被聚焦.
注意，这并不适用于所有情况，例如，当将数据输入到正在运行的应用程序时，导致它请求集中注意力。要在这种情况下配置行为，请参阅[聚焦到激活窗口](#4.28)
对于工作区中的第一个窗口，也不会忽略焦点，因为在这种情况下，不应该有理由不把焦点放在窗口上。这样就可以更好地结合工作空间的布局。
语法:

```
no_focus <criteria>
```

例子:

```
no_focus [window_role="pop-up"]
```

<h3 id="4.14">变量</h3>
当你学按键绑定时,有很多包含修改键.如果你想保存你的输入,并且在以后修改,变量就很方便.
语法:

```
set $<name> <value>
```

例子:

```
set $m Mod1
bindsym $m+Shift+r restart
```

在解析时变量直接替换ise个屏幕．依靠你的配置，i3将将新建的窗口放置在已有窗口的旁边或下面．
![](https://i3wm.org/docs/two_terminals.png)
将焦点在两个终端间移动，你能使用方向键，像使用vim/vi一样．然而，在i3里，你的homerow键（指打字时手指所放的准备位置）也被用于这些键．因此，$mod+j是左，$mod+k是下,$mod+l是上,$mod+;是右．所以，使用$mod+k或者$mod+l在两个终端间切换．当然也能用方向键．
现在你的工作空间在一个特殊的方向上分成两份（默认水平分）．每个窗口也能在一次被水平分或者垂直分，像工作空间一样．
垂直分割：$mod+v
水平分割：$mod+h
<h3 id="2.2">2.2.改变容器布局</h3>
一个分离容器能有以下任意一种布局：
splith/splitv
>窗口是有大小的，因此每个窗口在容器中有相同的空间．splith水平分割（窗口左右分布），splitv垂直分割（窗口上下分布）
>stacking(堆叠)
>只有目前聚焦的窗口在容器中显示．在容器上方显示窗口列表．
>tabbed
>原理和stacking相同，但窗口列表只是顶部的一条线
>![](https://i3wm.org/docs/modes.png)
>选择模式：
>splith/splitv:$mod+e
>stacking:$mod+s
>tabbed:$mod+w
><h3 id="2.3">2.3.切换窗口是否全屏</h3>
>使窗口全屏或者使全屏窗口恢复，按$mod+f.
>i3也有一个全局全屏模式，在这个模式客户端将跨越所有输出（命令是fullscreen toggle global)
><h3 id="2.4">2.4.打开其他软件</h3>
>除了从终端打开程序，你也可以使用方便的dmenu，默认用$mod+d打开dmenu．只要输入想要打开程序名称或一部分．相应的程序必须在PATH变量里．此外，如果你有些程序用得很频繁，你可以创建一个快捷键．详见[配置文件](#4)
><h3 id="2.5">关闭窗口</h3>
>如果程序没有提供一个关闭方式（大多数程序提供一个菜单，退出键或者ctrl+w快捷键来关闭），你可以用$mod+Shift+q来杀死一个窗口．对于提供WM_DELETE协议的程序，这将合理的关闭程序（存储任何修改，清除垃圾）．如果没有提供这个协议，你的X服务器将杀死窗口，这个行为依靠这个程序．
><h3 id="2.6">使用工作空间</h3>
>工作空间是一种把窗口组织起来的简单方式．默认是在第一个工作区间，它在底部状态栏左侧显示．切换到另一个工作区，按$mod+想切换到工作区的数字．如果它不存在，就会创建．
>如果你有多个屏幕，一个工作区将在开启时在每个屏幕上创建．如果你打开一个新的工作区，它将跳到你创建时的屏幕．当你切换到另一个屏幕上的工作区，i3将聚焦到那个屏幕
><h3 id="2.7">移动窗口到其他工作区</h3>
>只要按$mod+Shift+num将窗口移动到目标工作区．同样如果工作区不存在也会创建．
><h3 id="2.8">改变大小</h3>
>最简单的方法是用鼠标：拖边界到想到大小
>你也能用[捆绑模式](#4.5)去定义一个模式通过键盘改变大小．看一个简单的例子：看i3的[默认配置](https://github.com/i3/i3/blob/next/etc/config.keycodes)
><h3 id="2.9">重启i3</h3>
>重启i3可以使用$mod+Shift+r
><h3 id="2.10">退出i3</h3>
>干净的关闭i3而不杀死X服务器，你可以使用$mod+Shift+e.默认会弹出提示框让你确认．
><h3 id="2.11">悬浮模式</h3>
>悬浮模式和平铺模式相反．窗口的位置和大小不是被i3自动管理，而是由你手动管理．使用这个模式违反平铺，但对于一些小情形如＂保存为＂对话框，或者工具栏很有用．这种窗口通常设置适当的提示并默认以悬浮模式打开．
>你能使用$mod+Shift+Space将一个窗口切换到悬浮模式．通过鼠标用鼠标拖标题栏能四处移动窗口．拖动边缘能改变大小．也能通过[浮动修改器](#.4.6)做到这些．
><h2 id="3">树</h2>
>i3将所有关于X11输出、工作区和窗口布局的信息存储在树中.根节点是X11根窗口，紧接着是X11输出，然后是码头区域和一个内容集装箱，再然后工作区和窗口自己．在之前的i3版本中，我们有多个列表(输出、工作区)和每个工作区的表．这种方法被证明是复杂，难用，难以理解．
><h3 id="3.1">由容器组成的树</h3>
>树的构件叫做容器．容器能承载一个窗口（一个X11窗口）．另外，它包含一个或多个容器．一个简单的例子是工作区：但你在单屏幕打开i3，在一个工作区打开两个终端，最终你会得到一个这样的树：
>![](https://i3wm.org/docs/tree-layout2.png)
><h3 id="3.2">定位和分离容器</h3>
>在使用树作为数据结构时，使用所谓的分割容器是很自然的事情。每个容器都有一个定位(水平、垂直或未指明的方向)，而方向取决于容器的布局(垂直：splitv,stacking,水平:splith,tabbed).因此，在我们的工作空间示例中，工作区容器的默认布局是splith(现在大多数显示器都是宽屏).如果你把布局改变为splitv,然后打开两个终端，i3将配置你的桌面如下：
>![](https://i3wm.org/docs/tree-shot2.png)
>i3自版本４以来有一个有趣的新特性，就是能够分开任何东西：假使你有在同一个工作区两个终端（使用splith布局，水平定位），聚焦在右侧终端．现在如果你要打开另一个终端在现在这个终端的下面．如果你仅仅只是打开新的终端，由于splith布局的作用，新终端会在右侧．因此你需要按$mod+v切换布局到垂直模式．现在你就能在当前终端下方打开终端了．
>![](https://i3wm.org/docs/tree-shot1.png)
>![](https://i3wm.org/docs/tree-layout1.png)
>你也许早就猜到了：分裂等级的深度是没有限制的
><h3 id="3.3">聚焦到父级节点</h3>
>保持上一节的例子．左边有一个终端右边有两个垂直的分屏终端，焦点在右下方．当你打开一个新的终端时，它会在当前的这个终端下方打开．所以怎样在当前终端右侧打开呢？解决方案是使用focus parent(默认是$mod+a)这将聚焦到当前容器的父级容器．如果这样，您将聚焦到垂直分割容器，位于水平方向的工作区中．因此，现在新的窗口将在垂直分割的容器的右侧．
>ps:值得注意的是，垂直分割的容器的布局是splith
><h3 id="3.4">隐式容器</h3>
>在某些情况下，i3需要隐式地创建一个容器来实现您的命令。一个示例是这样的场景：您使用一个单独的显示器器启动i3，以及在其中打开三个终端窗口的单个工作区。所有这些终端窗口都直接连接到i3的布局树中的一个节点，即工作区节点。默认情况下，工作区节点的方向是水平的。
>现在你向下移动其中一个终端（默认是$mod+Shift+k）．工作空间节点的方向将被更改为垂直．您移动的终端窗口直接连接到工作区，并出现在屏幕的底部。创建了一个新的(水平的)容器，以容纳另外两个终端窗口。当切换到选项卡模式时，您就会注意到这一点.最后，您将得到一个带有拆分容器(例如“H[urxvt firefox]”)的标签，而另一个选项卡则是您移动的终端窗口。
><h2 id="4">配置i3</h2>
>这才是真正有趣的开始;-）。大多数东西都非常依赖于你理想的工作环境，所以我们不能为它们做出合理的默认设置.
>尽管没有用编程语言,i3对于一般窗口管理器所做的事也相当灵活.
>例如，您可以配置绑定快捷键来跳转到特定的窗口，您可以设置特定的应用程序以启动特定的工作空间，您可以自动启动应用程序，您可以更改i3的颜色，您可以绑定您的键来做有用的事情。
>改变i3的配置,复制/etc/i3/config到~/.i3/config(或者~/.config/i3/config,如果你喜欢XDG目录计划),并且用编辑器编辑它.
>第一次启动时(除非你已经有一个配置文件了),i3将提议你去创建一个配置文件.你可以告诉向导程序在配置文件中使用Alt(Mod1)或者Win(Mod4)作为mod键.同样,新建的配置文件将使用你目前的键盘布局.使用命令 i3-config-wizard打开向导程序.请确认你没有~/.i3/config文件,否则将退出引导程序.
>自i3 4.0以来,使用了一种新的配置文件格式.3将尝试基于几个不同的关键字自动检测配置文件的格式版本，但是如果你想确保你的配置是用新的格式读取的，那么在你的配置文件中包括以下一行:
```
# i3 config file (v4)
```
<h3 id="4.1">注释</h3>
可以在您的配置文件中使用注释来正确地记录您的设置，以便以后引用.注释是用#开头的，也只能在一行的开头使用:
例子:
```
# This is a comment
```
<h3 id="4.2">字体</h3>
i3支持X核心字体和自由字体（通过Pango）来渲染窗口标题.要生成X核心字体描述，您可以使用xfontsel(1).要查看特殊字符(Unicode)，需要使用支持iso-10646编码的字体.自由字体描述由字体家族、样式、重量、变体、拉伸和大小组成。FreeType字体支持从右到左的渲染，并且包含比X核心字体更多的Unicode字符.如果i3不能打开配置好的字体，它会在日志文件中输出一个错误，然后返回一个工作的字体.
语法:
```
font <X core font description>
font pango:<family list> [<style options>] <size>
```
例子:
```
font -misc-fixed-medium-r-normal--13-120-75-75-C-70-iso10646-1
font pango:DejaVu Sans Mono 10
font pango:DejaVu Sans Mono, Terminus Bold Semi-Condensed 11
font pango:Terminus 11px
```
<h3 id="4.3">按键绑定</h3>
键盘绑定使i3在按下特定键时执行命令(见下)。i3允许你在键码或键符号上绑定(你也可以混合你的绑定，不过i3不会保证你不重叠的).
+键符是一个特定的符号描述,像"a","b",但也有更奇怪的,像用"underscore"而不是"_".这是你在xmodemap中用来重新映射按键的符号.使用xmodmap -pke得到目前的键盘映射.要交互式地输入一个键并查看它被配置为什么键可以使用xev.
+键码不需要指定一个符号,当你切换到不同的键盘布局时(使用xmodmap)，它们不会改变它们的意思.
我的建议是:如果你经常切换键盘布局，但你想把你的绑定放在键盘上相同的物理位置上，使用键盘代码.如果您不切换布局，并且想要一个简洁且简单的配置文件，请使用键符.
有些工具(如import,xdotool)也许不能在按键事件上运行,因为键盘/鼠标指针仍然被占据.对于这种情形,可以使用--release标志,这将使命令在键被释放后执行.
语法:
```
bindsym [--release] [<Group>+][<Modifiers>+]<keysym> command
bindcode [--release] [<Group>+][<Modifiers>+]<keycode> command
```
例子:
```
# Fullscreen
bindsym $mod+f fullscreen toggle

# Restart
bindsym $mod+Shift+r restart

# Notebook-specific hotkeys
bindcode 214 exec --no-startup-id /home/michael/toggle_beamer.sh

# Simulate ctrl+v upon pressing $mod+x
bindsym --release $mod+x exec --no-startup-id xdotool key --clearmodifiers ctrl+v

# Take a screenshot upon pressing $mod+x (select an area)
bindsym --release $mod+x exec --no-startup-id import /tmp/latest-screenshot.png
```
可用修饰符:
Mod1-Mod5, Shift, Control ,Standard modifiers, 看 xmodmap(1)
Group1, Group2, Group3, Group4 
当你使用多个键盘布局(e.g. :  setxkbmap -layout us,ru),你可以指定哪个XKB组(或称布局)将被激活.默认按键绑定在Group1,并在所有组激活.如果你想在你的一个布局中重写键绑定,指定对应的组即可.对于向后兼容，组“Mode_switch”是Group2的别名.
<h3 id="4.4">鼠标绑定</h3>
鼠标绑定，在单击了的容器的范围内按下特定的鼠标按钮后使i3执行一个命令.您可以以类似于键绑定的方式配置鼠标绑定。
语法:
```
bindsym [--release] [--border] [--whole-window] [--exclude-titlebar] [<Modifiers>+]button<n> command
```
默认情况下，绑定只在单击窗口的标题栏时才会运行.如果给定了--release标志它将在鼠标按钮被释放时运行.
如果给定了 --whole-window标志,当窗口的任何部分除了边界之外被单击时，绑定也会运行.指定--border标志,在边界被点击时运行.
如果给定了--execlude-titlebar标签,标题栏不会包括进去.
例子:
```
# The middle button over a titlebar kills the window
bindsym --release button2 kill

# The middle button and a modifer over any part of the window kills the window
bindsym --whole-window $mod+button2 kill

# The right button toggles floating
bindsym button3 floating toggle
bindsym $mod+button3 floating toggle

# The side buttons move the window around
bindsym button9 move left
bindsym button8 move right
```
<h3 id="4.5">模式绑定</h3>
通过使用不同的绑定模式，您可以拥有多个绑定集.当您切换到另一个绑定模式时，当前模式下的所有绑定都将被释放，只有在新模式下定义的绑定才有效，只要您保持在这种绑定模式下.唯一的预定义绑定模式是默认模式，即i3开始时使用的模式，以及在特定绑定模式下没有定义的所有绑定.
绑定模式的工作由两部分组成:定义绑定模式并切换到绑定模式。出于这些目的，有一个配置指令和一个命令，这两个命令都被称为模式。该指令用于定义属于某个绑定模式的绑定，而命令用于切换到指定模式.
推荐使用[变量](#4.14)使维护更加容易.下面是一个如何使用模式绑定的例子.
注意:定义一个返回默认模式的绑定是明智的.
注意:可以使用[pango_markup]进行模式绑定,但必须模式定义时传入--pango_markup标记.
语法:
```
# config directive
mode [--pango_markup] <name>

# command
mode <name>
```
例子:
```
# Press $mod+o followed by either f, t, Escape or Return to launch firefox,
# thunderbird or return to the default mode, respectively.
set $mode_launcher Launch: [f]irefox [t]hunderbird
bindsym $mod+o mode "$mode_launcher"

mode "$mode_launcher" {
    bindsym f exec firefox
    bindsym t exec thunderbird

    bindsym Escape mode "default"
    bindsym Return mode "default"
}
```
<h3 id="4.6">悬浮修饰符</h3>
要用鼠标移动浮动窗口，你可以抓取它们的标题栏,或者配置所谓的浮动修饰符你可以点击并点击窗口的任何地方来移动它.最常见的设置是使用与管理windows相同的密钥（例如Mod1).然后你可以按下Mod1，用鼠标左键点击一个窗口，然后拖拽到你想要的位置.当你持有浮动的修改器时，你可以通过按下鼠标右键并再按住的同时移动来调整浮动窗口的大小.如果你按住shift键，那么调整的大小将是成比例的(相位比例将被保留).
语法:
```
floating_modifier <Modifier>
```
例子:
```
floating_modifier Mod1
```
<h3 id="4.7">限制悬浮窗口大小</h3>
可以指定浮动窗口的最大和最小尺寸.如果指定floating_maximum_size其中一个唯独指定为-1,这个维度将将没有最大值的限制.如果没有定义floating_maximum_size,或者指定为0,i3将使用默认的值限制窗口的最大值.floating_minimum_size也类似.
语法:
```
floating_minimum_size <width> x <height>
floating_maximum_size <width> x <height>
```
例子:
```
floating_minimum_size 75 x 50
floating_maximum_size -1 x -1
```
<h3 id="4.8">为新窗口定模式</h3>
新的工作空间得到合理的默认方向:宽屏显示器(宽大于高)得到水平方向,旋转了的屏幕(高大于宽)得到垂直方向.使用default_orientation配置指令，您可以覆盖该行为.
语法:
```
default_orientation horizontal|vertical|auto
```
例子:
```
default_orientation vertical
```
<h3 id="4.9">新容器的布局模式</h3>
该选项确定工作空间级别的新容器将在哪个模式下启动。
语法:
```
workspace_layout default|stacking|tabbed
```
例子:
```
workspace_layout tabbed
```
<h3 id="4,10">新窗口的边框样式</h3>
这个选项决定了新窗口的边界样式.默认值是normal.请注意，新的浮动只适用于windows，它是作为浮动窗口开始的，例如，对话框窗口，而不是稍后浮动的窗口.
语法:
```
new_window normal|none|pixel
new_window normal|pixel <px>
new_float normal|none|pixel
new_float normal|pixel <px>
```
例子:
```
new_window pixel
```
“正常”和“像素”边界样式支持一个可选的边框宽度:
例子:
```
# The same as new_window none
new_window pixel 0

# A 3 px border
new_window pixel 3
```
<h3 id="4.11">隐藏与屏幕边缘相邻的边框</h3>
您可以使用hide_edge_borders来隐藏与屏幕边缘相邻的容器边界.如果您使用滚动条，或者不想在显示空间中浪费两个像素，那么这非常有用."smart"设置在工作区只有一个窗口可见时隐藏边框,但在同一工作区多个窗口可见时不隐藏.默认是"none".
语法:
```
hide_edge_borders none|vertical|horizontal|both|smart
```
例子:
```
hide_edge_borders vertical
```
<h3 id="4.12">对于特定窗口的任意命令(for_window)</h3>
对于for_window命令,能让i3执行任何命令当它遇到指定窗口时.这可以用来设置窗口浮动或改变边框样式.
语法:
```
for_window <criteria> <command>
```
例子:
```
# enable floating mode for all XTerm windows
for_window [class="XTerm"] floating enable

# Make all urxvts use a 1-pixel border:
for_window [class="urxvt"] border pixel 1

# A less useful, but rather funny example:
# makes the window floating as soon as I change
# directory to ~/work
for_window [title="x200: ~/work"] floating enable
```
有效的标准与命令的标准是相同的
<h3 id="4.13">不聚焦到打开的窗口</h3>
no_focus命令能阻止一个新打开的窗口被聚焦.
注意，这并不适用于所有情况，例如，当将数据输入到正在运行的应用程序时，导致它请求集中注意力。要在这种情况下配置行为，请参阅[聚焦到激活窗口](#4.28)
对于工作区中的第一个窗口，也不会忽略焦点，因为在这种情况下，不应该有理由不把焦点放在窗口上。这样就可以更好地结合工作空间的布局。
语法:
```
no_focus <criteria>
```
例子:
```
no_focus [window_role="pop-up"]
```
<h3 id="4.14">变量</h3>
当你学按键绑定时,有很多包含修改键.如果你想保存你的输入,并且在以后修改,变量就很方便.
语法:
```
set $<name> <value>
```
例子:
```
set $m Mod1
bindsym $m+Shift+r restart
```
在解析时变量直接在文件中替换.变量扩展不是递归的，因此不可能用包含另一个变量的值定义一个变量.没有什么奇特的处理方式，而且绝对没有改变这种情况的计划.如果您需要一个更动态的配置，您应该创建一个小脚本，该脚本生成一个配置文件，并在启动i3之前运行它.还可以看到[xresources](#4.15)学习如何基于从X资源数据库加载的资源创建变量.
<h3 id="4.15"> X resources</h3>
还可以使用在X资源数据库中配置的值创建变量。这是很有用的，例如，避免在i3配置中配置颜色值。相反，这些值可以在X资源数据库中配置一次，以便在许多X应用程序中实现易于维护的、一致的颜色主题。定义资源将从资源数据库中加载该资源，并将其值分配给指定的变量。必须指定一个回滚，以防资源不能从数据库中加载。
语法:
```
set_from_resource $<name> <resource_name> <fallback>
```
例子:
```
# The ~/.Xresources should contain a line such as
#     *color0: #121212
# and must be loaded properly, e.g., by using
#     xrdb ~/.Xresources
# This value is picked up on by other applications (e.g., the URxvt terminal
# emulator) and can be used in i3 like this:
set_from_resource $black i3wm.color0 #000000
```
<h3 id="4.16">自动将客户端放到指定工作区</h3>
为了使指定的窗口在指定的工作区展示,可以使用一个assignment.你可以用任意条件匹配窗口.建议匹配窗口类(和实例，适当的时候)而不是窗口标题，因为一些应用程序首先创建它们的窗口，然后担心设置正确的标题.Firefox聚焦到Vimperator网站.窗口开始被命名为Firefox，只有当Vimperator被加载时，标题才会改变.当应用程序映射到窗口时（映射意味着在屏幕上显示它），当i3得到这个标题时，你需要在这个例子中匹配Firefox.assignment由i3按配置文件中的顺序处理.只处理匹配的第一个,后面的不被考虑.
语法:
```
assign <criteria> [→] [workspace] <workspace>
```
例子:
```
# Assign URxvt terminals to workspace 2
assign [class="URxvt"] 2

# Same thing, but more precise (exact match instead of substring)
assign [class="^URxvt$"] 2

# Same thing, but with a beautiful arrow :)
assign [class="^URxvt$"] → 2

# Assignment to a named workspace
assign [class="^URxvt$"] → work

# Start urxvt -name irssi
assign [class="^URxvt$" instance="^irssi$"] → 3
```
注意，箭头不是必需的，它看起来很好:-)。如果你决定使用它，它必须是一个utf-8编码的箭头，不是->或者类似的东西.
要获得类和实例，您可以使用xprop.单击该窗口之后，您将看到以下输出:
xprop
```
WM_CLASS(STRING) = "irssi", "URxvt"
```
WM类的第一部分是实例(在本例中是“irssi”)，第二部分是类(在本例中是“URxvt”).
如果你使用assignment报错,请务必首先检查i3日志文件(看[make sure to ](https://i3wm.org/docs/debugging.html)).它包含了关于匹配过程的更多细节，以及窗口的实际类、实例和标题.
注意，如果您想在特定的工作空间上只启动一次应用程序，但是您不希望永久地分配它的所有实例，那么您可以在配置文件中使用i3的启动通知支持（见exec）：
Start iceweasel on workspace 3 (once):
```
# Start iceweasel on workspace 3, then switch back to workspace 1
# (Being a command-line utility, i3-msg does not support startup notifications,
#  hence the exec --no-startup-id.)
# (Starting iceweasel with i3’s exec command is important in order to make i3
#  create a startup notification context, without which the iceweasel window(s)
#  cannot be matched onto the workspace on which the command was started.)
exec --no-startup-id i3-msg 'workspace 3; exec iceweasel; workspace 1'
```
<h3 id="4.17">在i3启动时自动开始程序</h3>
通过在keybinding之外使用exec关键字，您可以配置在初始启动时，i3将执行哪些命令。在重新启动i3时，exec命令不会运行，如果您需要在重新启动i3时运行的命令，那么应该使用exec_always关键字。这些命令将按顺序运行。
语法:
```
exec [--no-startup-id] <command>
exec_always [--no-startup-id] <command>
```
如果要执行的命令包含一个;(分号)和/或,(逗号),则必须引用整个命令.比如你有一个快捷shell命令notify-send Hello, i3,您可以在配置文件中添加一个条目:
例子:
```
# Execute a command with a comma in it
bindsym $mod+p exec "notify-send Hello, i3"
```
如果一个带有逗号和/或分号的命令需要引号，那么您必须使用双反斜杠来转义内部引号，如下:
例子:
```
# Execute a command with a comma, semicolon and internal quotes
bindsym $mod+p exec "notify-send \\"Hello, i3; from $USER\\""
```
<h3 id="4.18">自动将工作区放到指定屏幕</h3>
如果您将客户分配到工作区，那么将工作区放在特定的屏幕上是很方便的。此外，当添加屏幕或开始时，对屏幕的工作空间分配将决定i3在新屏幕上使用的是哪个工作区(例如，默认情况下，它将在第一个屏幕上使用1，第二个屏幕是2，等等)。
语法:
```
workspace <workspace> output <output>
```
output是您将屏幕连接到的RandR输出的名称.在一台笔记本电脑上，可能会有VGA1和LVDS1作为输出名称.你可以通过运行xrandr --current查看可用输出.
如果您的X服务器支持RandR 1.5或更新，那么i3将使用RandR监视器对象，而不是输出对象。运行 xrandr --listmonitors去看列表.通常，监视器对象只包含一个输出，并且具有与输出相同的名称;但如果不是这种情况，您可以指定i3配置中的监视器或输出的名称。例如，戴尔UP2414Q在内部使用了两个标量，因此它的输出名可能是“DP1”和“DP2”，但监视器名称是“Dell UP2414Q”.
(请注意，即使您指定了一个输出的名称，该输出没有覆盖整个监视器，但是i3仍然会使用包含监视器的整个区域，而不是输出的内容.)
如果你使用已经命名的工作空间,就必须引用他们.
例子:
```
workspace 1 output LVDS1
workspace 5 output VGA1
workspace "2: vim" output VGA1
```
<h3 id="4.19">改变颜色</h3>
你可以改变所有的颜色，用i3来装饰窗口.
语法:
```
<colorclass> <border> <background> <text> <indicator> <child_border>
```
colorclass可以是以下其中一个:
client.focused:目前聚焦的客户端
client.focused_inactive:被聚焦的容器中目前不被聚焦的客户端
client.unfocused:目前不聚焦的客户端
client.urgent:一个有紧急提示的被激活的客户端
client.placeholder:背景和文本颜色用于绘制占位符窗口内容(在恢复布局时)。边界和指示器被忽略。
client.background:背景颜色，将用于绘制客户端窗口的背景，客户端将在其中显示客户端窗口。只有不覆盖整个窗口的客户机才会显示颜色。注意，这个颜色类只需要一个颜色。
颜色以HTML十六进制格式(#rrggbb)，请参见下面的示例:
例子(默认颜色):
```
# class                 border  backgr. text    indicator child_border
client.focused          #4c7899 #285577 #ffffff #2e9ef4   #285577
client.focused_inactive #333333 #5f676a #ffffff #484e50   #5f676a
client.unfocused        #333333 #222222 #888888 #292d2e   #222222
client.urgent           #2f343a #900000 #ffffff #900000   #900000
client.placeholder      #000000 #0c0c0c #ffffff #000000   #0c0c0c

client.background       #ffffff
```
注意，对于窗口装饰，子窗口周围的颜色是“子边界”，而“边框”颜色只是标题栏周围的两条细线.
指示符颜色用于指示新窗口将在哪里打开。对于水平分割容器，正确的边界将被涂成指示色，用于垂直分割容器，底部边界。这只适用于拆分容器内的单个窗口，这与拆分容器外的单个窗口是无法区分的。
<h3 id="4.20">进程通讯</h3>
i3使用Unix套接字来提供IPC接口。这允许第三方程序从i3获得信息，比如当前的工作空间（显示工作空间条），以及控制i3.
IPC套接字默认启用，将在/tmp/i3-%uxxxxxx/IPC-socket中创建。%p%u是您的UNIX用户名，%p是i3的PID和XXXXXX是可移植的文件名字符集的一串随机字符(参见mkdtemp(3)).
您可以通过环境变量I3SOCK或指定ipc-socket指令来覆盖默认路径.不过，这是不鼓励的，因为i3在默认情况下是正确的.如果您决定更改它，强烈建议将其设置为您的主目录中的一个位置，这样就没有其他用户可以创建该目录了.
例子:
```
ipc-socket ~/.i3/i3-ipc.sock
```
然后可以使用i3-msg应用程序执行下一节中列出的任何命令。
<h3 id="4.21">跟随鼠标聚焦</h3>
默认情况下，当鼠标经过窗口边界时，窗口焦点会跟随鼠标移动。但是，如果你有一个设置，你的鼠标通常在你的方向上(比如你的笔记本上的一个触摸板，你不想完全禁用)，你可能想要禁用鼠标和控制焦点，只需要使用你的键盘。
在当前活动窗口中，鼠标仍然是有用的（例如，单击您的浏览器窗口中的链接）。
语法:
```
focus_follows_mouse yes|no
```
例子:
```
focus_follows_mouse no
```
<h3 id="4.22">鼠标扭曲</h3>
默认情况下，当将焦点切换到另一个输出的窗口时(例如，在输出vga1上聚焦一个窗口，从lvds-1的工作区2开始)，鼠标指针会被扭曲到该窗口的中心.
有了mouse_warping选项，你就可以控制鼠标光标的位置了.none将完全禁用调整，而output是上面描述的默认行为.
语法:
```
mouse_warping output|none
```
例子:
```
mouse_warping none
```
<h3 id="4.23">全屏时弹出框模式</h3>
当你处于全屏模式时，一些应用程序仍然会打开弹出窗口(比如Xpdf)。这是因为这些应用程序可能没有意识到它们处于全屏幕模式(它们没有检查相应的提示)。在这种情况下，有三件事是可以做到的:
>1.如果它只属于全屏幕应用程序，就显示它.对于大多数用户来说，这是默认的，应该是合理的行为.
>2.忽略弹出窗口(不要映射它).当你在全屏时，这不会打断你.然而，一些应用程序可能会对此做出严重的反应(死锁直到你离开了全屏).
>3.退出全屏
语法:
```
popup_during_fullscreen smart|ignore|leave_fullscreen
```
例子:
```
popup_during_fullscreen smart
```
<h3 id="4.24">焦点封装</h3>
当您在一个选项卡或堆叠的容器中，当您将焦点放在最后一个容器上时，第一个容器将会聚焦在焦点包装上。如果在那个方向有另一个堆叠/标签的容器，那么焦点就会集中在那个容器上。这是默认行为，这样您就可以导航到所有的窗口，而不必使用焦点节点。 如果您希望焦点始终封装，并且您知道使用焦点的父元素切换到不同的容器，那么您可以使用force_focus_wrapping配置指令。在启用它之后，焦点总是会结束。
语法:
```
force_focus_wrapping yes|no
```
例子:
```
force_focus_wrapping yes
```
<h3 id="4.25">强制多屏幕</h3>
作为https://i3wm.org/docs/multi-monitor.html深入解释,一些X11视频驱动程序(尤其是nVidia二进制驱动程序)只提供支持Xinerama代替RandR。在这种情况下，i3必须被告知要显式地使用劣质的Xinerama API，因此不能提供对重新配置屏幕的支持(它们只在启动时被读取一次，仅此而已).
对于不能在~/.xsession添加 --force-xinerama参数的人,提供一个配置选项:
语法:
```
force_xinerama yes|no
```
例子:
```
force_xinerama yes
```
还需要注意的是，当使用Xinerama时，你的输出名不是描述性的(比如HDMI1)，而是从0开始，从0开始: xinerama-0, xinerama-1, …
<h3 id="4,26">切换到当前工作区时自动来回切换</h3>
例如：假设您在工作空间“1:www”，然后切换到“2:IM”，使用mod 2，因为有人给您发送了一条消息。你不需要记住你从哪里来，你只需按下$mod+2，就可以切换回“1:www”.
语法:
```
workspace_auto_back_and_forth yes|no
```
<h3 id="4.27">在工作空间更改上延迟紧急提示</h3>
如果在另一个工作空间上的应用程序设置了紧急提示，切换到这个工作空间可能会导致应用程序的立即焦点，这也意味着窗口的装饰颜色会立即被重置为client.focus。这可能会让你很难分辨哪个窗口最初是由哪个窗口引起的.
为了防止这种情况发生，你可以告诉i3，在一定时间内延迟重置紧急状态,使用force_display_urgency_hint参数.将值设置为0将禁用该特性.默认是500ms.
语法:
```
force_display_urgency_hint <timeout> ms
```
例子:
```
force_display_urgency_hint 500 ms
```
<h3 id="4.28">专注激活窗口</h3>
如果一个窗口被激活，例如，通过google-chrome www.google.com，它可能会要求集中注意力.由于这可能不是更好的选择，所以可以配置不同的反应.注意，这可能不会影响正在打开的窗口。为了防止新窗口被关注，请不要关注焦点.
语法:
```
focus_on_window_activation smart|urgent|focus|none
```
不同的模式将如下:
smart:这是默认行为。如果请求焦点的窗口位于活动工作区，则它将接收焦点。否则，紧急提示将被设定
urgent:窗户总是被标记为紧急的，但是焦点不会被偷走。
focus:窗口将始终保持焦点，而不被标记为紧急
none:窗户既不会被聚焦，也不会被标记为紧急
<h3 id="4.29">在窗口装饰绘制标记</h3>
如果被激活，在窗口上的标记被画在窗口的装饰上。但是，即使在该选项被激活时，任何以下划线开头的标记()都不会被绘制.
默认是yes
语法:
```
show_marks yes|no
```
<h3 id="4.30">续行符</h3>
配置文件支持行延续，这意味着当您在反斜杠字符(\)中结束一行时，换行符会被解析器忽略。该特性可用于创建更可读的配置文件。注释行没有继续
例子:
```
bindsym Mod1+f \
fullscreen toggle

# this line is not continued \
bindsym Mod1+F fullscreen toggle
```
<h2 id="5">配置i3bar</h2>
在你的显示器底部的bar是由一个叫做i3bar的单独的过程画出来的。在一个单独的进程中拥有“i3用户界面”的这一部分有几个优点:
>1.这是一种模块化的方法。如果您根本不需要工作空间栏，或者您想要一个不同的工作空间（dzen2、xmobar，甚至是gnome-panel），那么您只需删除i3bar配置并启动您最喜欢的工具条即可。
>2.它遵循了UNIX的“使每个程序都能做一件事”的哲学。虽然i3能够很好地管理你的窗口，但是i3bar可以很好地在每个监视器上显示一个栏（除非你对它进行了配置）.
>3.它会导致两个独立的、干净的代码库。如果你想了解i3，你不需要去关注i3bar的细节，反之亦然。
也就是说，i3bar配置在与i3相同的配置文件中。这是因为它与i3紧密耦合(与i3lock或i3status相反，这对使用其他窗口管理器的人很有用)。因此，当我们已经有了良好的配置基础设施时，使用不同的配置位置是毫无意义的。
配置您的工作空间bar从打开一个bar块开始。您可以有多个bar块来为不同的输出使用不同的设置(监视器):
例子:
```
bar {
    status_command i3status
}
```
<h3 id="5.1">i3bar命令</h3>
默认情况下，i3只是通过i3bar让你的shell处理执行，搜索你的$PATH，找到正确的版本。如果你在某个地方有一个不同的i3bar，或者二进制不在你的$PATH中，你可以告诉i3要执行什么。
指定的命令会传递给sh -c,因此你可以用文件名代替,但必须有正确的引用
语法:
```
Y
```
<h3 id="5.2">状态栏命令</h3>
i3bar可以运行一个程序，并在栏的右侧显示其输出的每一行输出。这有助于显示系统信息，如当前IP地址、电池状态或日期/时间.指定的命令会传递给sh -c,因此你可以用文件名代替,但必须有正确的引用.注意，对于信号处理，取决于您的shell(dash(1)的用户会受到影响)，您必须使用shell的exec命令，以便将信号传递给您的程序，而不是shell。
语法:
```
status_command <command>
```
例子:
```
bar {
    status_command i3status --config ~/.i3status.conf

    # For dash(1) users who want signal handling to work:
    status_command exec ~/.bin/my_status_command
}
```
<h3 id="5.3">显示模式</h3>
你可以让i3bar永久地出现在屏幕的一个边缘(dock模式)，或者当你按你的修改器键(隐藏模式)时显示它。也有可能迫使i3bar始终隐藏(不可见的模式)。修改器键可以使用修饰符选项进行配置.
模式选项可以在运行时通过bar模式命令更改。在重新加载模式时，模式将被恢复到它的配置值
隐藏模式使可用于实际窗口的屏幕空间最大化。同样，i3bar向statusline发送SIGSTOP和SIGCONT信号以节省电量。
不可见的模式允许永久地最大化屏幕空间，因为条形图从未显示。因此，您可以配置i3bar以避免由于紧急提示或因为修饰符键被按下而弹出
与模式一样，隐藏状态也可以通过i3进行控制，这可以通过使用bar_state状态命令来实现
默认模式是dock模式;在隐藏模式下，默认的修饰符是Mod4(通常是windows键)。隐藏状态的默认值是隐藏的。
语法:
```
mode dock|hide|invisible
hidden_state hide|show
modifier <Modifier>|none
```
例子:
```
bar {
    mode hide
    hidden_state hide
    modifier Mod1
}
```
可用的修饰符是mod1-mod5，Shift，Control（参见xmodmap（1））。如果您不希望任何修饰符触发此行为，您也可以使用“none”。
<h3 id="5.4">鼠标键命令</h3>
指定在i3bar上按下一个按钮来覆盖默认行为的命令。这很有用，例如，可以禁用滚动轮操作或为这些按钮实现自定义行为的脚本。
一个按钮总是被命名为button<n>，其中1到5个是默认的按钮，更高的数字可以是提供更多按钮的设备上的特殊按钮：
button1

    Left mouse button.
button2

    Middle mouse button.
button3

    Right mouse button.
button4
    滚轮向上转
button5
    滚轮向下转
    
注意:wheel_up_cmd和wheel_down_cmd不宜使用,将在未来的版本被移除.我们强烈建议使用绑定button4和button5代替

语法:
```
bindsym button<n> <command>
```
例子:
```
bar {
    # disable clicking on workspace buttons
    bindsym button1 nop
    # execute custom script when scrolling downwards
    bindsym button5 exec ~/.i3/scripts/custom_wheel_down
}
```
<h3 id="5.5">Bar ID</h3>
为配置的bar实例bar ID.如果没有定义这个选项,ID会被设置为bar-x,x对应于配置中块的位置(bar-0, bar-1, …).
语法:
```
id <bar_id>
```
例子:
bar {
    id bar-1
}
<h3 id="5.6">位置</h3>
这个选项决定了i3bar屏幕的哪边应该显示出来。 默认是底部。
语法:
```
position top|bottom
```
<h3 id="5.7">输出</h3>
您可以将i3bar限制为一个或多个输出（监视器）。默认情况是处理所有输出。限制输出对于使用多个bar块来为不同的输出使用不同的选项是很有用的。要让一个特定的i3bar实例处理多个输出，可以多次指定输出指令。
语法:
```
output primary|<output>
```
例子:
```
# big monitor: everything
bar {
    # The display is connected either via HDMI or via DisplayPort
    output HDMI2
    output DP2
    status_command i3status
}

# laptop monitor: bright colors and i3status with less modules.
bar {
    output LVDS1
    status_command i3status --config ~/.i3status-small.conf
    colors {
        background #000000
        statusline #ffffff
    }
}

# show bar on the primary monitor and on HDMI2
bar {
    output primary
    output HDMI2
    status_command i3status
}
```
注意，您可能还没有配置一个主输出。为此,运行:
```
xrandr --output <output> --primary
```
<h3 id="5.8">托盘输出</h3>
i3bar默认提供了一个系统托盘区域，其中网络管理器、VLC、Pidgin等程序可以放置小图标.您可以配置哪个输出（监视器）图标应该显示，或者您可以完全关闭该功能.
你可以在你的配置中使用多个tray_output指令来指定一个你想要显示托盘的输出列表。按照指令的顺序定义的列表中的第一个可用输出将用于托盘输出.
语法:
```
tray_output none|primary|<output>
```
例子:
```
# disable system tray
bar {
    tray_output none
}

# show tray icons on the primary monitor
bar {
    tray_output primary
}

# show tray icons on the big monitor
bar {
    tray_output HDMI2
}
```
请注意，当您使用多个bar配置块时，要么在所有这些块中指定tray_output primary，要么显式地指定tray_output none，而不应该显示托盘，否则不同的实例可能会在试图显示托盘图标时相互竞争。

<h3 id="5.9">托盘垫</h3>
这个托盘在bar的右手边。默认情况下，在托盘区域的上、下、右端使用2个像素的填充，并在各个图标之间使用。
语法:
```
tray_padding <px> [px]
```
例子:
```
# Obey Fitts's law
tray_padding 0
```
<h3 id="5.10">字体</h3>
语法:
```
font <font>
```
例子:
```
bar {
    font -misc-fixed-medium-r-normal--13-120-75-75-C-70-iso10646-1
    font pango:DejaVu Sans Mono 10
}
```
<h3 id="5.11">定制的分割符号</h3>
指定用于分隔符的自定义符号而不是垂直的,一个像素厚分离器.
语法:
```
separator_symbol <symbol>
```
例子:
```
bar {
    separator_symbol ":|:"
}
```
<h3 id="5.12">工作区按钮</h3>
指定工作空间按钮是否应该显示。如果您想要显示一个仅包含其他信息的状态栏，那么这是非常有用的.默认是显示.
语法:
```
workspace_buttons yes|no
```
<h3 id="5.13">去除工作区数字</h3>
指定工作区号是否应该显示在工作区按钮中。如果您想要在没有显示数字前缀的情况下，根据它的编号来保持一个命名的工作区，那么这是非常有用的。
当strip_workspace_numbers设置为yes,任何具有“n:name”形式名称的工作空间都只显示名称。例如，你可以用这个来显示罗马数字而不是数字，通过给你的工作区命名为“1:I”，“2:2”，“3:3”，“4:IV”。
默认显示全名
语法:
```
strip_workspace_numbers yes|no
```
<h3 id="5.14">绑定模式指示器</h3>
指定当前的绑定模式指示器是否应该显示。如果您想要隐藏工作空间按钮，但仍然能够看到当前的绑定模式指示器，这是非常有用的。请参阅绑定模式以了解何种模式以及如何使用它们。
默认是显示
语法:
```
binding_mode_indicator yes|no
```
<h3 id="5.15">颜色</h3>
和i3一样，颜色是用HTML十六进制格式(#rrggbb)。现在可以配置以下颜色：
background
>bar背景色
statusline
>状态栏文字颜色
separator
>分隔符颜色
focused_background 
>当前聚焦的监视器输出的背景颜色。如果不使用，颜色将从background中提取。
focused_statusline 
>当前聚焦的监视器输出的状态栏文字颜色。如果不使用，颜色将从statusline中提取
focused_separator 
>同上理
focused_workspace
>当工作区有焦点时，工作区按钮的边框、背景和文本颜色
active_workspace 
>当工作区处于活动状态（可见）时，工作区按钮的边框、背景和文本颜色会显示在某些输出上，但重点放在另一个输出上。当您使用多个监视器时，您只能从集中的工作区中区分这一点。
inactive_workspace 
>当工作空间没有焦点时，工作区按钮的边框、背景和文本颜色，并且在任何输出上都不是活动的(可见的)。对于大多数工作空间来说都是这样。
urgent_workspace 
>当工作区包含一个带有紧急提示集的窗口时，工作区按钮的边框、背景和文本颜色。
binding_mode 
>绑定模式指示器的边框、背景和文本颜色。如果不使用，颜色将从urgent中取出
语法:
```
colors {
    background <color>
    statusline <color>
    separator <color>

    <colorclass> <border> <background> <text>
}
```
<h2 id="6">命令列表</h2>
