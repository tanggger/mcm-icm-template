## 参考文献的插入以及引用
### 一、参考文献的格式

latex中参考文献的格式需要设置为`BibTeX`

### 二、怎么在LaTex中插入参考文献

在`tex`文件同目录下创建一个`bib`文件

在`tex`文件的倒数第二行加两行代码，注意`bibliography`的参数要与`bib`文件名一致，代码位置如下：

~~~tex
\bibliographystyle{plain}%按作者姓氏排序
\bibliographystyle{unsrt}%按添加顺序排序
%上面两个二选一
\bibliography{reference}
~~~

在`tex`文件正文里引用格式为`\cite{}`，注意大括号里的参数要与`bib`文件里的参考文献别名一样。

### 三、怎么实现点击参考文献号跳转到对应参考文献

在导包的地方加一行代码后，文献引用号码会变颜色，点击号码就可以跳转到对应的参考文献。

~~~tex
\usepackage{hyperref}
~~~
