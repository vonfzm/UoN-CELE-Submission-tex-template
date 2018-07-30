# UoN-CELE-Submission-tex-temple
A TeX temple for University of Nottingham CELE students,to help them with their submissions' fromat  
Because most of CELE students are Chinese,This readme will be written in Chinese. 
  
这个TeX模版是为诺丁汉大学CELE（读音为silly）的学生准备，由于学校要求统一格式，较为繁琐，如果你希望仅输入纯文本即可自动输出排版好的论文，并且格式与美观均可保证的话，那么本模版将大大简化你的写作过程。本模版有详细的使用教程，作为一个接受过九年义务教育的你，请不必担心读不懂它。 但是如果你还不知道如何用word进行排版，请务必学会，以免日后与我不在一个学院时无法继续使用这项服务。请务必提前开始写，因为如果交作业前一天再来看本教程，将会面临ddl所引起的不必要恐慌，难以从可能面临的各种问题中实现自我救赎。如果你有任何问题，欢迎致信fzm@mail.ustc.edu.cn
  
本模版遵守以下格式：  
-----------------
1. 使用Verdana字体（虽然这是一个非衬线字体，且为商业字体，但学校为学生免费提供）  
2. 使用10号字  
3. 行间距为2倍字号（为了方便老师批注）  
4. 段间空一行  
5. 页边距为2.5cm  
6. 使用Harvard文献引用与列表格式（References大号居中标题经老师证明符合要求）
7. 在封面页最上方添加校徽以免封面太过单薄（符合学校官网对logo使用的要求，即使用时充满自豪感、完整、与背景不冲突，并经过老师证明符合要求）
8. 页码从正文开始，并延伸到参考文献页
  
使用方法：
-------
1. 配置TeX环境：  
详见[中国科学技术大学学位论文LaTeX模板新手指南](https://github.com/ustctug/ustcthesis/wiki/%E6%96%B0%E6%89%8B%E6%8C%87%E5%8D%97)，本project不再赘述。
2. 下载本模版：  
下载地址：  
下载到的应该是一个zip，将其解压，~~洗干净切丁~~备用
3. 使用编辑器打开temple.tex  
4. 输入基本信息，26到31行为封面页信息，依次为题目、作者、班级、提交时间、学科（我写了CELE）、字数（如何统计将在下文中给出）。只需将这六行中大括号内内容改为你自己的即可，标题过长也会有自动换行与对齐，请不必担心。
5. 输入正文：  
正文从53行开始，夹在`\begin{flushleft}`与`\end{flushleft}`之间，段落之间
