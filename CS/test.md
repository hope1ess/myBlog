# 一级标题
## 二级标题
### 三级标题
标题就是用卸载'#'后面
>这个是引用的方法 >
# 插入链接
[跳转到链接](http:://www.baidu.com)
![图片](https://upload-images.jianshu.io/upload_images/703764-605e3cc2ecb664f6.jpg?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
分割线
***
加粗**两个**
斜体*一个*
***
表头|一|二
:---:|:---:|:---:
项目一|项目二|项目三
***
```c++
    #include <iostream>
    using namespace std;
    int main()
    {
        int a, b, flgA, flgB, pa = 0, pb = 0;
        cin >> a >> flgA >> b >> flgB;
        while (a != 0)
        {
            if (a % 10 == flgA) pa = pa * 10 + flgA;
            a = a / 10;
        }
        while (b != 0)
        {
            if (b % 10 == flgB) pb = pb * 10 + flgB;
            b = b / 10;
        }
        cout << pa + pb << endl;
        system("pause");
        return 0;
    }
```
test in emacs