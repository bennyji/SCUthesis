# 四川大学硕博学位论文LaTaX模板SCUthesis
## --对标研究生院硕博论文格式2010年版
## 0 写在前面
本人为四川大学电气工程学院的研究僧，在毕业论文也使用LaTeX，在Legendary Leo同学的scuthesis模板基础上，参照研究生院官网的模板2010版的进行多处修改完善，最后制作了适用于硕博同学的本模板，暂命名为SCUthesis v1.0beta。
由于本人部分实现差异产生的瑕疵，欢迎大家指出，通过留言、新建一个ISSUSE或FORK一个新分支修改。最最后，这是本人在Github发布的第一个项目，希望对大家有所帮助。

#### 本项目对应的overleaf链接（不推荐在线使用，就模板生成结果来看，页面会有点问题，声明处的四川大学也没法显示，推荐直接下载本项目本地进行修改）：https://cn.overleaf.com/read/bypstqfsnqwd
#### 文档效果图 
![xiaoguotu](https://github.com/bennyji/SCUthesis/tree/master/Manual/Images/封面目录.png)
![xiaoguotu2](https://github.com/bennyji/SCUthesis/tree/master/Manual/Images/正文声明等.png)
## 1 概述
### 1.1 模板基础
本LaTeX模板是在Legendary Leo 于2016年的四川大学学位论文模板[1]的基础上进行修改的。而Legendary Leo的四川大学学位论文模板[1]的工作，以前由 dahakawang  、 tan  等人做过，是在参考 Casper Ti. Vector   pkuthss 模版的基础上完成的。在此一并感谢。
### 1.2 适用人群
本模板适用于四川大学硕博毕业生学位论文写作，不推荐本科生不做修改的前提直接使用（要求有所不一样）。
### 1.3 推荐配置
笔者具体的配置其实忘记了（不要打我），只是遇到一个问题解决一个，大致的需要以下一些要求：

•	中文支持：我貌似暗装的CTeX，支持中文。

•	编辑器：个人推荐TeXstudio，界面功能都很不错。

##### 附上一个不错的环境配置的博客（可以按这个教程配置环境）：https://blog.csdn.net/aijava1/article/details/99282235

### 1.4 文件夹列表及说明
      因为太长了，所以放在最后。

## 2 本模板特点与改进
首先在继承Legendary模板简单方便与自动化程度高的特点的基础上，高度符合《四川大学硕士、博士学位论文格式（2010版）》[2]。对原版本主要进行了以下几个方面的修改：


### (1)版面修改:
    16k正度（国内尺寸）：185x260，版心: 145x215mm

### (2)字号相关修改:
    将一级标题强制设置为小三号大小，同时修改参考文献为五号；
    摘要中专业改为小四号宋体并将“专业”两字后置，将“关键字”三个字设为小四黑体.

### (3)页码相关修改:
    封面页之后开始进行罗马数字编号，目录页紧接着进行罗马数字编号，去除多余空白页；
    去除了目录中的目录【在不包含缩略词表和符号表的情况下，目录中不含“目录”从正文开始；
    若有两个表则会从该表开始出现】。

### (4)参考文献内容样式的修改:
    尝试了多个.bst文件之后，选择了清华大学模板中[3]的.bst文件 。
    英文文献时，作者名首字母大写，姓只保留首字母大写；
    中文多作者用“等”，英文多作者用“et al”。符合国标。
    该.bst文件后被修改为本项目中的"scuthesis-bythu.bst"文件。

### (5)英文摘要处的修改:
    删掉了“Presented for MSc Degree”，将“Subject”改为了“Major”。

### (6)其他可能因学院细化要求的修改:
        一级标题居左排，样式为“1 绪论”；页眉为“四川大学硕士学位论文”居中
        （注：本处可以根据学院要求和个人喜好进行修改。
        如果有同学采用“第x章”的形式有可能会遇到目录中字重叠现象，
        也是可以搜索解决，或根据MainBody.tex相关注释操作。）
## 补充：文件夹列表及说明（对应1.4）

* -README.md（自述文件）

* -Lincenses（许可文件夹）
    * fdl-1.3.txt
    * gpl-3.0.txt {这两个具体干啥的，我也不知道，主要是从原模板中复制过来的}
* -MainBody（论文主体文件夹）
    * MainBody.tex      {主TeX文件}.
    * ReferenceBase.bib      {参考文献库文件}.
    * Chapters      {章节文件夹}.
        * 0_0_Abstract.tex      {中英文摘要}.
        * 0_1_Abbreviations.tex      {缩略词表}.
        * 0_2_Symbols.tex      {符号表}.
        * 1_Introduction.tex      {引言}.
        * 2_Theory      {第二章}.
        * 3_Methods      {第三章}.
        * 4_Results      {第四章}.
        * 5_Summary      {第五章}.
        * Thanks.tex      {致谢}.
        * Achievements.tex      {科研成果}.
        * CopyrightAuthorization.tex      {版权授权（请勿修改）}.
        * OriginalStatement.tex      {原创声明（请勿修改）}.   
 
* -Manual（手册文件夹）
    * Manual.tex      {手册说明主TeX文件}.
    * Manualbib.bib      {手册参考文献库文件}.
        * CopyrightStatement.tex      {声明}.
        * 0_0_Abstract.tex      {中英文摘要}.
        * 1_Introduction {前言}.
        * 2_Changing{改进与说明}
        * 3_Using{说明文档}
        * 4_Realization{部分功能实现}
        * 5_Updating{更新记录} 
        * Thanks.tex      {致谢}.
        * Achievements.tex      {科研成果}.
        * CopyrightAuthorization.tex      {版权授权（请勿修改）}.
        * OriginalStatement.tex      {原创声明（请勿修改）}.   
* -Reference Document（参考文献文件夹）
    * pkuthss-1.2beta {参考模板文件夹}.
    * scuthesis2016 {scu模板文件夹}.
    * 四川大学硕士、博士学位论文格式.doc {word版参考文件}.
* -Template（模版文件夹）
    * scuthesis.cls {模版样式文件}.
    * scuthesis.def {模版宏定义文件}.
    * chinesebst.bst {中文参考文献样式文件，模板未使用}.
    * scuthesis-bythu.bst{符合要求的参考文献样式文件，使用的版本}
    * Components.
        * Images.
            * SCU_TITLE.eps {四川大学LOGO}.

## 3 参考文献与项目
[1] LegendaryLeo. 四川大学学位论文LaTeX模版 Poweredbypkuthss-1.2beta[EB/OL].
2016[2020.03.04]. https://github.com/cuiao/SCU_ThesisDissertation_LaTeXTemplate.

[2] 四川大学研究生院. 四川大学硕士、博士学位论文格式2010[2020.03.24][EB/OL]http://gs.scu.edu.cn/__local/5/12/88/D4DE41B158E85CFA0705D213A24_39BC1820_C400.doc?e=.doc

[3] 焦润之. LaTeX Thesis Template for Tsinghua University.[2020.03.24][EB/OL]https://gitee.com/jiaorzh/thuthesis. 
