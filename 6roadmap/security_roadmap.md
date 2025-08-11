## 📌技术学习路线-安全岗

#### 1. 整体而言

   网络安全领域中细分方向很多，从就业岗位来说主要有以下三个方向：
- 安全研发
- 安全研究：<font color=Blue>二进制安全方向</font>
- 安全研究：<font color=Blue>web渗透安全方向</font>
  
每个方向下还有细分领域。除了以上三个大方向之外，还有如云安全、AI安全、工控安全、可信计算、身份认证等细分方向。
 ![](/6roadmap/security-fields.png)

网络安全有哪些方向，它们之间有什么关系和区别，以及各方向学习路线更详细的内容可以参考：
  - http://cnblogs.com/hack4396/p/16063151.html
  - https://www.freebuf.com/articles/web/270481.html


#### 2. 偏实战或是偏研究

时间充裕的情况下，渴望从事安全领域建议从CTF起手。时间不充裕不建议走安全方向。🤓

- 实战方向
   - 线上实践 ：在*CTFSHOW*(https://ctf.show/)平台，可以根据方向去做Web安全、逆向工程、二进制漏洞利用（PWN）、密码学、取证分析等方向的题目，这样基本掌握了常见漏洞。
  
   - 护网行动：多找机会参加hw行动，教育hw也可以。
  
   - 认证证书：如果资金充裕，可以选择看一下*Offsec*（https://www.offsec.com/courses/ ）的*OSCP*和*OSEP*两个认证证书；如果资金不充裕，可以网上购买这两个的教材跟着学，但没有Lab和考试。
    
     ps： 关于*Offsec*证书认证（*OSCP*、*OSEP*、*OSWE*、*OSED*四大认证对比，看这一篇就够了！https://blog.csdn.net/weixin_43766412/article/details/127610686 ）。
  
   - 网络靶场：可以选择*Hack The Box*（https://www.hackthebox.com/ ）靶场进行打靶学习；*TryHackMe*（https://tryhackme.com/ ）有非常完善的教学，跟学基本够用。*SRC*漏洞挖掘，可以从教育*SRC*开始，之后再到专属*SRC*，可以从*HackerOne*的公开报告中学习。
  
    
- 研究方向：例如：*Java*安全研究；安全产品：*Webshell*、*WAF*之类的检测；云安全：*K8S*、*AWS*等等。


#### 2. 以二进制安全为例，<font color=orange>入门学习路线</font>
| 主题        | 详细描述 |
| :---------- | :------- |
|汇编语言	| - 学习amd32，amd64汇编语言，能够做到识别基础汇编指令，理解汇编语言的运行逻辑；<br>- 若有能力可以进一步了解arm，mips等架构的汇编语言。|
|Linux基础|	如题|
|JAVA基础|- JAVA语法基础；<br> - 了解JNI(Java Native Interface)|
|C/C++语言基础| - 能够使用C语言写简易脚本； <br> - C语言中，分支，循环，函数调用(普通函数，函数指针，类函数，虚函数，递归)的汇编实现；<br> - 在二进制文件中，函数局部变量，拥有初始值的全局变量，未拥有初始值的全局变量，静态变量，局部静态变量等的区别； <br> - C语言函数调用约定，__cdecl，__stdcall，__fastcall，理解“调用者保存寄存器”与“被调用者保存寄存器”，理解栈帧结构；<br>  - C语言中常见寄存器的使用，例：在x86架构中，EAX（32位）和在x86-64架构中的RAX（64位）通常用来存储函数的返回值；<br>  - C++中class的内存布局，继承&多态的汇编实现；<br>   - C语言中常见数据存储方式，大小端序区别，整数溢出影响，强制类型转换原理(int $\rightarrow$ long long；long long $\rightarrow$ int等)；<br> - 指针、引用的汇编实现；<br>  - 构造函数，构析函数，复制函数，移动构造函数的调用时机（特别是当作函数参数传递时）；<br>  - 静态编译与动态编译的编译产物的区别，动态编译的编译产物的运行原理。
|python语言基础&python逆向知识|	- 部分库使用python，需熟练使用python。例：angr。<br> - python常见的pyc、pyd文件逆向。
|PE文件结构&ELF文件结构|了解即可|
|常见编码&古典加解密&现代加解密&哈希算法|- base64（以及其衍生），凯撒密码，替换密码，维吉尼亚密码，栅栏密码；<br> - DES，AES，TEA，RC4，RSA，MD5，SHA-1，SHA-256，简易字符串哈希（https://oi-wiki.org/string/hash/ ）|
|常见数据结构与算法|- 链表、单链表、双向链表、循环链表（增、删、查、改操作）、图论等； <br> - 最短路径算法（Dijkstra，Floyd，SPFA）；<br> - 深度优先搜索、广度优先搜索（部分CTF需要爆破答案）......
|代码混淆/保护|- OLLVM项目，指令替换，混淆控制流，控制流平坦化；<br> - 花指令，SMC技术，壳技术，虚拟机代码保护；<br> - 原理与反混淆思路。
|安卓逆向|- 安卓生态基本了解，安卓开发基础了解；<br> - Dalvik字节码和 ART字节码；<br> - 安卓获取root(实体机，虚拟机均可)；<br> - firda，Unidbg工具使用。|
|调试技术|- 普通断点，硬件断点（架构相关）原理；<br> - 常见反调试技术，inline hook检测技术；<br> - inline hook技术原理与使用。
|其余常用工具&库|Cheat Engine|