###计算机基础知识(常见的DOS命令讲解)
* d: 回车	盘符切换
* dir(directory):列出当前目录下的文件以及文件夹
* cd (change directory)改变指定目录(进入指定目录)
* cd.. : 退回到上一级目录
* cd\: 退回到根目录
* cls : (clear screen)清屏
* exit : 退出dos命令行(分割线上的需要掌握,下的了解)
* /=========================================================
* md (make directory) : 创建目录
* rd (remove directory): 删除目录
* del (delete): 删除文件,删除一堆后缀名一样的文件*.txt
* notepad 创建文件
* 删除带内容的文件夹
	* rd + /s	文件夹名称(询问是否删除)
	* rd + /q + /s 文件夹名称(直接删除)


###Java语言基础
* Java语言平台
	* J2SE(Java 2 Platform Standard Edition)标准版
		* 是为开发普通桌面和商务应用程序提供的解决方案,该技术体系是其他两者的基础，可以完成一些桌面应用程序的开发
	* J2ME(Java 2 Platform Micro Edition)小型版
		* 是为开发电子消费产品和嵌入式设备提供的解决方案
	* J2EE(Java 2 Platform Enterprise Edition)企业版
		* 是为开发企业环境下的应用程序提供的一套解决方案,该技术体系中包含的技术如 Servlet、Jsp等，主要针对于Web应用程序开发 

* Java语言特点
	* 简单性		
	* 解释性
	* 面向对象		
	* 高性能
	* 分布式处理	
	* 多线程
	* 健壮性		
	* 动态
	* 结构中立		
	* 安全性
	* 开源
	* 跨平台


* Java语言跨平台原理
	* 只要在需要运行java应用程序的操作系统上，先安装一个Java虚拟机(JVM Java Virtual Machine)即可。由JVM来负责Java程序在该系统中的运行。
	* write once ,run anywhere!(一处编译,到处运行)

* JRE和JDK的区别
	* JRE：包括Java虚拟机(JVM Java Virtual Machine)和Java程序所需的核心类库等，如果想要运行一个开发好的Java程序，计算机中只需要安装JRE即可
	* JDK：提供给Java开发人员使用，其中包含了java的开发工具，也包括了JRE。所以安装了JDK，就不用在单独安装JRE了。

* JDK安装路径下的目录解释
	* A:bin目录：该目录用于存放一些可执行程序。
		* 如javac.exe（java编译器）、java.exe(java运行工具)，jar.exe(打包工具)和* javadoc.exe(文档生成工具)等。
	* B:db目录：db目录是一个小型的数据库。
		* 从JDK 6.0开始，Java中引用了一个新的成员JavaDB，这是一个纯Java实现、开源的数据库管理系统。这个数据库不仅轻便，而且支持JDBC 4.0所有的规范，在学习JDBC 时，不再需要额外地安装一个数据库软件，选择直接使用JavaDB即可。
	* C:jre目录："jre"是 Java Runtime Environment 的缩写，意为Java程序运行时环境。此目录是Java运	行时环境的根目录，它包括Java虚拟机，运行时的类包，Java应用启动器以及一个bin目录，但不包含开	发环境中的开发工具。
	* D:include目录：由于JDK是通过C和C++实现的，因此在启动时需要引入一些C语言的头文件，该目录就是用	于存放这些头文件的。
	* E:lib目录：lib是library的缩写，意为 Java 类库或库文件，是开发工具使用的归档包文件。
	* F:src.zip文件：src.zip为src文件夹的压缩文件，src中放置的是JDK核心类的源代码，通过该文件可以	查看Java基础类的源代码。

###第一个Java程序(HelloWorld案例的编写和运行)
* A:定义类
* B:写main方法
* C:写输出语句
* D:Java程序开发运行与工作原理
* E:编译和运行程序

		class HelloWorld {
			public static void main(String[] args) {
				System.out.println("HelloWorld");
			}
		}

###Java语言的书写格式(约定俗成)
* A,大括号要对齐,并且成对写
* B,左大括号前面有空格
* C,遇到左大括号要缩进,Tab
* D,方法和程序块之间加空行让程序看起来清晰
* E,并排语句之间加空格,例如for语句
* F,运算符两侧加空格

###Java注释概述及其分类
*   单行注释  // 注释内容
*   多行注释  /* 注释内容 */
*   文本注释  /** 注释内容 */

###Java关键字
* 关键字：被Java语言赋予特定含义的单词
* 特点：组成关键字的字母全部小写
* 常见关键字：public static void class等
* 关键字的注意事项：goto和const作为保留字存在,目前并不使用

###标识符的概述和组成规则
* 标识符：给类,接口,方法,变量等起名字时使用的字符序列
* 标识符的组成规则
	* 英文大小写字母
	* 数字字符
	* $和_
* 标识符注意事项
	* 不能使用关键字
	* 不能数字开头 
	* 不能使用（$和_）外的特殊字符
*标识符中常见的命名规则
	* 见名知意
	* A:包
		* 最好是域名倒过来,要求所有的字母小写 
	* B:类或者接口
		* 如果是一个单词首字母大写
		* 如果是多个单词每个单词首字母大写(驼峰标识) 
	* C:方法或者变量
		* 如果是一个单词全部小写
		* 如果是多个单词,从第二个单词首字母大写 
	* D:常量
		* 如果是一个单词,所有字母大写
		* 如果是多个单词,所有的单词大写,用下划线区分每个单词 
