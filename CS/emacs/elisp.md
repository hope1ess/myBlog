在elisp中，关键字nil为假，其他任何值为真，t为真

用=去比较有局限性，可以用关键字equal代替

Emacs中的变量无需声明，作用域为全局，用setq给变量赋值，形如
``` lisp
(setq x 1) ;; x赋值为1
(setq x 1 y 2 z 3) ;; 多重赋值
```

在emacs中定义一个函数，形如
```lisp
(defun function()
    "testing"
    (message "ya"))
```
与在scheme中定义函数稍有出入，调用函数的方式相同。
emacs中函数返回最后的表达式。

在emacs中的函数如果想在M-x中调用，则需要在函数中加入 (interactive)
```lisp
(defun yay()
  (interactive)
  (insert "yay!"))
```
如此便能在M-x中调用yay命令