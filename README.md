# jemdoc-resume

demo: https://jemnz.com/
![alt text](images/demo.jpg "title")

## 生成网页
index.jemdoc ----> index.html
```
$ python2 jemdoc.py index.jemdoc
```

## 语法说明
1. http://jemdoc.jaboc.net/
2. https://github.com/jem/jemdoc

例如：

添加菜单 - http://jemdoc.jaboc.net/menu.html

jemdoc provides an easy way to add a ‘menu’ like the one you see at the left of this page. You should create a file called MENU, for example, in the current directory. This website's MENU looks something like this:
```
jemdoc
    home                [index.html]
    download            [download.html]
    revision history    [revision.html]
    contact             [contact.html]

user's guide
    cheat sheet         [cheatsheet.html]
    using               [using.html]

goodies
    add a menu          [menu.html]
    other stuff         [stuff.html]
```
To use the menu, start the first line of each source file with a special comment like this one:
```
# jemdoc: menu{MENU}{index.html}
```
(Replace index.html with the name of the relevant html page.) This will add a menu from the file called MENU, and underline and darken the menu entry corresponding to index.html.
