# 基本语法以及语义
>定义函数
``` scheme
;;a的平方
(define (squart a) (* a a))
```
函数的代换模式分为**正则序**和**应用序**
>cond,直到找到第一个true
```scheme
(define (abs x)
  (cond ((= x 0) 0)
        ((> x 0) x)
        ((< x 0) (- x))))
```
术语**谓词**指返回真或假的过程
