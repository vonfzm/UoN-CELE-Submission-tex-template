# 说明文档
Because most of CELE students are Chinese,in order to prevent students from facing additional language barriers during using,this readme will be written in Chinese.But I have translated it to English.[Click here to view English version](#english-version)  

由于大多数同学是中国人，为了避免学生在使用过程中额外面临语言障碍，本说明文档将以中文书写。但我也已将其翻译为英语。[点击此处阅读英文版](#english-version)  
  
这个TeX模版是为诺丁汉大学CELE（读音为silly）的学生准备的，由于学校要求统一格式，较为繁琐，如果你希望仅输入纯文本即可自动输出排版好的论文，并且格式与美观均可保证的话，那么使用本模版将大大简化你的写作过程。本模版有详细的使用教程，作为一名接受过九年义务教育的优秀共产主义接班人，你大可不必担心读不懂它。 但是如果你还不知道如何用word进行排版，请务必学会，以免形成依赖但日后与我不在一个学院而无法继续使用这项服务时出现无助感。如果你决定使用但没有TeX基础的话，请务必提前开始着手，因为如果交作业前一天晚上再来看本教程，将会面临ddl所引起的不必要恐慌，从而难以从可能面临的各种问题中实现自我救赎。如果你有任何问题，欢迎致信fzm@mail.ustc.edu.cn
  
本模版严格遵守以下格式：  
-----------------
1. 使用10号Verdana字体（虽然这是一个非衬线字体，且为商业字体，但学校思路清奇审美独特，且已经购买了正版并为学生免费提供。）  
2. 行间距为2倍字号（为了方便老师批注）  
3. 段落之间空一行  
4. 页码从正文开始，并延伸到参考文献页  
5. 页边距为2.5cm  
6. 对齐方式为justify  
7. 根据学校邮件要求，使用考文垂大学规定的Harvard文献引用与列表格式（References大号标题经老师证明符合要求） 
8. 在封面页最上方添加校徽以免封面太过单薄（符合学校官网对logo使用的要求，即使用时充满自豪感、完整、与背景不冲突，并经过老师证明符合要求）
  
参考文献及所询问的老师：
---------------
1. [USE OF HARVARD REFERENCING，The University of Nottingham, School of Education](https://dokumen.tips/documents/use-of-harvard-referencing.html)(Version 2.0 - 22.03.2013)
2. [The Coventry University Guide to Referencing in Harvard Style Guidelines and Glossary](https://www.coventry.ac.uk/Documents/Lanchester%20Library/Guide%20to%20Referencing%20in%20Harvard%20Style%20Version%204.0%20September%202017.pdf)(Version 4.0 September 2017)
3. [Submission 2 - Details (Course Texts booklet)](http://moodle.nottingham.ac.uk/pluginfile.php/4542903/mod_folder/content/0/Submission%202%20-%20Details%20%28Course%20Texts%20booklet%29.docx?forcedownload=1)   
4. Katerina Liontou <alzkl@exmail.nottingham.ac.uk>
5. Robito Chatwin <alzrc@exmail.nottingham.ac.uk>

使用方法：
-------
1. 配置TeX环境：  
详见[中国科学技术大学学位论文LaTeX模板新手指南](https://github.com/ustctug/ustcthesis/wiki/%E6%96%B0%E6%89%8B%E6%8C%87%E5%8D%97)，本project不再赘述。

2. 下载本模版：  
下载地址：https://github.com/vonfzm/UoN-CELE-Submission-tex-template/files/2260784/template.zip
下载到的应该是一个zip，将其解压，~~洗净切丁，沾上鸡蛋清，裹上面包糠炸至两面金黄~~备用  

3. 打开源文件：  
使用编辑器（Mac上为TexShop，Windows上可能为TexWorks或WinEdt）打开`template.tex  `。  

4. 输入基本信息：  
26到31行为封面页信息，依次为题目、作者、班级、提交时间、学科、字数（如何统计将在下文中给出）。只需将这六行中大括号内内容改为你自己的即可，标题过长也会有自动换行与对齐，请不必担心。  

5. 输入正文：  
正文从53行开始，在`\newpage`之前结束（你可以无限回车使`\newpage`无限往下，行数没有任何限制）。换段用`\par`。  

6. 参考文献的引用：  
首先用文献管理软件(在Mac上为BibDesk）打开下载好的文件夹中`bibliography.bib `。然后在谷歌学术中找到你将引用的参考文献，点击它下面的引号，你将看到引用界面，此时我们点击左下角第一个BibTeX，得到一堆代码，全选，复制，粘贴到我们的文献管理软件中。然后选中它，软件会提供复制引用命令，或者你手动输入引用命令。请注意，我们被要求使用Harvard格式，在不同情况下需要有不同引用风格，所以请将默认引用命令`\cite{}`根据需要改为你所需要的指令（如下表） 

| 引用指令       |           效果 |
| ------------- | ------------- |
| \citet{jon90}  |Jones et al. (1990)  |
| \citet[chap.~2]{jon90}  | Jones et al. (1990, chap. 2)  |
| \citep{jon90}  | (Jones et al., 1990)  |
| \citep[chap.~2]{jon90}  | (Jones et al., 1990, chap. 2)  |
| \citep[see][]{jon90}  | (see Jones et al., 1990)  |
| \citep[see][chap.~2]{jon90}  | (see Jones et al., 1990, chap. 2)  |
| \citet*{jon90}  | Jones, Baker, and Williams (1990)  |
| \citep*{jon90}  | (Jones, Baker, and Williams, 1990)  |
| \citet{jon90,jam91}  | Jones et al. (1990); James et al. (1991)  |
| \citep{jon90,jam91}  | (Jones et al., 1990; James et al. 1991)  |
| \citep{jon90,jon91}  | (Jones et al., 1990, 1991) |
| \citep{jon90a,jon90b}  | (Jones et al., 1990a,b)  |
| \citeauthor{jon90}  | Jones et al.  |
| \citeauthor*{jon90}  | Jones, Baker, and Williams  |
| \citeyearpar{jon90}  | (1990)  |
| \citealp[pg.~32]{jon90}  | Jones et al., 1990, pg. 32  |
  
7. 插入整段quotation（如果需要的话）：  
在以下两行命令之间插入你的quotation  
`\begin{quotation}`   
`\end{quotation}`    

8. 编译：  
我们一共需要四次编译（也有编译器叫做排版），第一次用XeLaTeX，这是编译你的.tex文件，这时生成一个.aux的文件, 这告诉BibTeX将使用哪些引用。接下来用BibTeX编译。再次用XeLaTeX编译, 个时候在文档中已经包含了参考文献, 但此时引用的编号可能不正确。最后用XeLaTeX编译你的.tex文件，如果一切顺利的话，这时所有东西都已正常了。  
（请注意，根据编辑器不同，做法也有不同，比如CTex F9 可以一次性编译完成，TexShop需要选方法按四次排版，而有的编译器还需要第二次换成对.bib文件进行排版）
  
9. 字数统计：  
在终端（Mac在启动台-其它中找，Windows为Win+R，跳出来的窗口中输入cmd，回车）中，首先输入`cd 你的template文件夹的路径`，比如放在桌面就是`cd Desktop\template`然后输入`texcount template.tex`，就会显示出正文、标题各有多少字，且参考文献不会算在字数里。 
  
10. 转成Word格式（__很重要！__）：  
由于我们的老师只会用Microsoft Word进行批注（事实上这也是学校买正版的原因），所以我们需要把得到的PDF转成Word文档。  
使用Adobe Acrobat打开你得到的PDF文件，左上角菜单，文件-导出到-Microsoft Word-Word 文档，重命名并导出即可。  
你也可以使用其它方式进行这种转换，但Adobe作为PDF格式的提供者，Acrobat作为官方PDF阅读与编辑工具，似乎更加稳妥。  
  
避免出现错误食用方法：
--------
1. 请不要使用中文或任何数学公式，包括全角标点符号。  
2. 请不要下载后把其中的PDF转成docx再写！那样写出来的作业是没有灵魂的！就像用擦丝器生产土豆丝一样不可饶恕！  
3. 如果出现报错请先百度或Google，这种简单的纯英语论文基本上都是常见问题。如果再不行，再顺着网线来砍我（这种做法不被提倡）。。。。   
4. 请不要事先吓自己，心态要平稳。因为这个并不比word难用，只是你可能还未熟悉。  

致谢：
----
1. 感谢提供LaTeX指导的[@Zeping Lee](https://github.com/zepinglee)、Johannes Gutenberg以及Chinese TeX User Group telegram组全体成员  
2. 感谢提供格式指导的Katerina Liontou老师与Robito Chatwin老师  
3. 感谢提供协助的黄娇雅同学、王俪霓同学、黄馨逸同学。

# ReadMe  

A TeX template for University of Nottingham CELE students,to help them with their submissions' fromat  
  
This TeX template is for students of the University of Nottingham CELE. Because the school requires a uniform format, it is kinds of cumbersome. If you want to input only plain text, and automatically output the typeset paper, with the format and appearance guaranteed,then by using this template, you will greatly simplify your writing process. This template has a detailed tutorial, you don't have to worry about understanding it. But if you have not known how to typeset with word, make sure to learn it to avoid reliance, or you will feel helpless when you are not in the same faculty with me and can't continue to use this service in the future. If you decide to use but don't have a TeX foundation, start early. Because if you look at this tutorial the night before deadline, you will face unnecessary panic caused by ddl, making it difficult to achieve self salvation from the various problems you may face. If you have any questions, don't hesitate to contact me at fzm@mail.ustc.edu.cn  
  
This template strictly adheres to the following format:
-------
1. Verdana size 10 font(though Verdana is a sans serif font,and commercial product as well,but our university is supplying it to us for free)   
2. 2 line spacing(for teachers to add comments)  
3. an empty line between paragraphs  
4. page numbers from text to references  
5. standard margins (2.5cm)  
6. justify  
7. Harvard literature citation and list format as specified by Coventry University according to requirements in the mail sent by school  
8. Add the school badge at the top of the cover page to avoid the cover being too thin (in accordance with the school's official website requirements for logo use, which is using it proudly, completeness, and not conflicting with the background)

References and Teachers I refered to:
-------
1. [USE OF HARVARD REFERENCING，The University of Nottingham, School of Education](https://dokumen.tips/documents/use-of-harvard-referencing.html)(Version 2.0 - 22.03.2013)
2. [The Coventry University Guide to Referencing in Harvard Style Guidelines and Glossary](https://www.coventry.ac.uk/Documents/Lanchester%20Library/Guide%20to%20Referencing%20in%20Harvard%20Style%20Version%204.0%20September%202017.pdf)(Version 4.0 September 2017)
3. [Submission 2 - Details (Course Texts booklet)](http://moodle.nottingham.ac.uk/pluginfile.php/4542903/mod_folder/content/0/Submission%202%20-%20Details%20%28Course%20Texts%20booklet%29.docx?forcedownload=1)   
4. Katerina Liontou <alzkl@exmail.nottingham.ac.uk>
5. Robito Chatwin <alzrc@exmail.nottingham.ac.uk>  

Instructions:
------
1. Configuring the TeX environment:  
please refer to [University of Science and Technology University Dissertation LaTeX Template Beginner's Guide](https://github.com/ustctug/ustcthesis/wiki/%E6%96%B0%E6%89%8B%E6%8C%87%E5%8D%97)，This project will not describe again.  
  
2. Download this template:  
Download link：https://github.com/vonfzm/UoN-CELE-Submission-tex-template/files/2260784/template.zip
You will get a zip，unzip it. 
  
3. Open the source code file:  
Use editor（TexShop on Mac，TexWorks or WinEdt on Windows）to open `template.tex  `.  
  
4. Input your information:  
The information on cover sheet is from line 26 to 31，it's title、author、class、date、academic subject、word count（How to statist will be given below）.Fill in your information in the curly braces，If the title is too long, there will be automatic line breaks and alignment，please don't worry.  
  
5. Input your text:  
The text begins from line 53，ends before `\newpage`.Use `\par` to begin a new paragraph.  
  
6. Cite references:  
First open the `bibliography.bib` in the downloaded folder with the document management software (BibDesk on Mac). Then find the reference you will quote in Google Scholar, click on the quotation marks below it, you will see the reference interface, at this point we click on the BibTeX in the lower left corner, get a bunch of code, select all, copy, paste to the .bib file  in the document management software. Then select it, the software will provide a copy cite command, or you can manually enter the reference command. Please note that we are required to use the Harvard format, which requires different reference styles in different situations, so please change the default reference command \cite{} to the one you need (as shown below).

| command       |           result |
| ------------- | ------------- |
| \citet{jon90}  |Jones et al. (1990)  |
| \citet[chap.~2]{jon90}  | Jones et al. (1990, chap. 2)  |
| \citep{jon90}  | (Jones et al., 1990)  |
| \citep[chap.~2]{jon90}  | (Jones et al., 1990, chap. 2)  |
| \citep[see][]{jon90}  | (see Jones et al., 1990)  |
| \citep[see][chap.~2]{jon90}  | (see Jones et al., 1990, chap. 2)  |
| \citet*{jon90}  | Jones, Baker, and Williams (1990)  |
| \citep*{jon90}  | (Jones, Baker, and Williams, 1990)  |
| \citet{jon90,jam91}  | Jones et al. (1990); James et al. (1991)  |
| \citep{jon90,jam91}  | (Jones et al., 1990; James et al. 1991)  |
| \citep{jon90,jon91}  | (Jones et al., 1990, 1991) |
| \citep{jon90a,jon90b}  | (Jones et al., 1990a,b)  |
| \citeauthor{jon90}  | Jones et al.  |
| \citeauthor*{jon90}  | Jones, Baker, and Williams  |
| \citeyearpar{jon90}  | (1990)  |
| \citealp[pg.~32]{jon90}  | Jones et al., 1990, pg. 32  | 
  
7. Insert an entire paragraph of quotation（if needed）:  
Insert your quotation between this two lines of command. 
`\begin{quotation}`   
`\end{quotation}` 
  
8. Type:
We need to type a total of four times, the first time with XeLaTeX, this is to compile your .tex file, then generate a .aux file, which tells BibTeX which references to use. Next compile with BibTeX. Compiling with XeLaTeX again, the reference is already included in the documentation, but the number referenced at this time may be incorrect. Finally, compile your .tex file with XeLaTeX. If everything goes well, then we have completed.
(Please note that depending on the editor, the methods are different. For example, CTex can be compiled in one click(F9), TexShop needs to select the method to type four times, and some compilers need to switch to .bib file for the second time.)  
 
9. Word count:
In the terminal (on Mac you can find it in the lunchpad - other, on Windows,press Win + R, input cmd in the window that pops up and press enter), first input `cd "path of your template folder" `, such as on the desktop,it's `cd Desktop\template` .Then enter `texcount template.tex`, which will display the number of words in the body and title, and the words in references will not be counted.   
  
10. Convert your PDF to .docx(__very important!__):   
Because our teachers will only use Microsoft Word for comments,so we need to convert the pdf document to MS word format.
Open the PDF file you get with Adobe Acrobat, the top left menu, File - Export to - Microsoft Word-Word document, rename and export.
You can also use other methods to do this conversion, but sicne Adobe is the offical PDF provider, Acrobat is the official PDF reading and editing tool,it seems to be more secure.    
  
