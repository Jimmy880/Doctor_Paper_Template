华南理工大学学位论文Latex/Lyx模板
=============================

【主要特色】
----------

*   至今第一个专业型华南理工大学Latex论文模板
*   全国高校论文模板中，首创支持Lyx论文编辑
*   模板使用与操作系统平台无关，一键生成pdf文件
*   框架简洁高效，适宜作为其他高校Latex／Lyx论文模板设计的母版

【设计概要】
----------

本设计包括两部分：latex模板类和lyx模板布局，书写文档时使用其一即可。其流程框架、模板使用和文件关系如图1。

latex模板类包括文本布局类scutthesis.cls和参考文献样式scutthesis.bst。
采用XeLATEX排版引擎编辑方式使用Unicode编码克服多种字体带来麻烦。在传统的Tex使用方式中（way 1），
先用Tex编辑器直接输入你的论文内容(参照例子scutthesis.tex格式)，再运行xelatex，
其调用scutthesis.cls和scutthesis.bst就可以格式化为符合华南理工大学学位论文的排版要求。注意摘要之前的几页排版内容，
如标题和版权页，是以pdf文件方式包括在tex文件中，发布包中提供了相应word的.doc版文件，请自行修改再转换为pdf文件。

你也可以通过lyx间接地使用latex模板类（图中way 2），不需要直面latex源代码。
在lyx中采用scutthesis.layout布局，输入你的论文内容如scutthesis.lyx格式，
再一键调用xelatex自动编译成scutthesis.tex文件，并加入scutthesis.cls和scutthesis.bst生成最终的pdf文件。


【适用对象】
----------

所有能够运行Latex的系统，和所有能够运行lyx的系统（可选）

1.    Linux(ubuntu)测试过的环境为Texlive2009+lyx；
2.    Windows测试过的环境为Ctex + miktex+lyx；
3.    MAC OS X测试过的环境为Mactex2011+Lyx2.0。


【使用简介】
----------

使用之前先确认安装好Xelatex以及必要的中文字体，Lyx软件推荐安装。详见scutthesis.pdf相关章节。

*   用lyx打开论文模板文件scutthesis.lyx,调用xelatex菜单项或者工具栏按钮编译即可，最终生成scutthesis.pdf文件。
*   如果你的lyx未能调用xelatex，那么用lyx将scutthesis.lyx导出为latex plain格式的scutthesis.tex，再用Texmarker+xelatex编译。
*   调用用户的 scutthesis.bib 文件，lyx中有相关设置界面，属于lyx使用的问题；
*   你的论文可以从修改thesis_cover.doc和scutthesis.lyx而来。
