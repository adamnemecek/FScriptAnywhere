F-Script Anywhere for Mac OS X Mavericks (10.9), Yosemite (10.10), El Capitan (10.11)
===============

##Description##
This repository contains an updated F-Script Anywhere Automator workflow compatible with Mac OS X Mavericks. In Mavericks, GDB was retired and therefore this workflow uses LLDB instead. The original F-Script Anywhere for Snow Leopard was written by Silvio H. Ferreira.

##What is F-Script?##
[F-Script](https://en.wikipedia.org/wiki/F-Script_\(programming_language\)) is a Smalltalk inspired programming language. F-Script's runtime can be injected into running processes and allows for interactive exploration of running processes. It is therefore a great tool e.g. for debugging or reverse engineering.
You can see F-Script in action [here](http://www.youtube.com/watch?v=SNVnoulAHbg).

##How to install##
You have to have F-Script installed in order to use this workflow (install from [here](http://www.fscript.org/download/download.htm)). After unpacking the F-Script zip file, copy the `FScript.framework` to `/Library/Frameworks`. Then install this workflow. After launching an application into which you want to inject F-Script, open the main application menu, select `Services` and click `Inject_FScript` as shown on the image below.

![inject_fscript](https://raw.github.com/adamnemecek/FScriptAnywhere/master/pic1.png)

A new item `F-Script` should appear on the top menu bar as shown on the image below. You can then launch the F-Script environment.

![inject_fscript](https://raw.github.com/adamnemecek/FScriptAnywhere/master/pic2.png).

##Other considerations##
For whatever reason the F-Script console treats the input of a single straight quotation mark `'` as a curved unicode quotation mark `‘`. In order to input e.g. a string literal (which is in F-Script delimited by two single straight quotation marks), one must input the straight quotation mark using a key combination `control` + `'`.

__Update__(Jul 23, 2015): It appears that the quote issue has been fixed in [recent versions of F-Script](https://github.com/Kentzo/F-Script/releases).
