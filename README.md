thupagescan
====

本宏包为使用[ThuThesis](https://github.com/xueruini/thuthesis)撰写的清华大学学位论文提供扫描页替换功能，并保证生成的PDF文档中书签和页码的正确性。

本宏包依赖于`xkeyval`和`pdfpages`宏包。


使用方法
----

1.  将`thupagescan.sty`置于`main.tex`所在目录。
2.  在`main.tex`中引入本宏包。使用示例如下。

    ```latex
    \usepackage[final,
        path=scanned/,
        authpage=authorization.pdf,
        declpage=declaration.pdf,
        formfront=form-front.pdf,
        formback=form-back.pdf
    ]{thupagescan}
    ```


选项说明
----

 *  `final` - 指定是否使用扫描页替换论文中相应部分内容。使用`final`或`final=true`打开该选项；使用`final=false`或删除`final`关闭该选项（即不替换扫描页）。
 *  `path` - PDF扫描页所在目录。
 *  `authpage` - 《关于学位论文使用授权的说明》扫描页文件名。
 *  `declpage` - 论文致谢部分《声明》扫描页文件名。
 *  `formfront` - 本科《综合论文训练记录表》扫描页正面文件名。
 *  `formback` - 本科《综合论文训练记录表》扫描页反面文件名。
