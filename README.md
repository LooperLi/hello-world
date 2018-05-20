# hello-world
a single repository
msi i hope rng can win the kzoom
lazyman1111111

一：
    1）文本编译器
     notepad
	 
    2）编译器
    GCC
	安装：http://gcc.gnu.org/install/ 
	windows： www.mingw.org 下载最新版本的 MinGW 安装程序，命名格式为 MinGW-<version>.exe
	
二：程序结构
    1）关键字
	--四种存储类别--
	auto；register 自动存储期
	extern；static 静态存储期
	
	--逻辑判断-----
	if  else
	do  while
	switch case  default break
	for continue
	goto
	return
	
	
	--数据类型定义--
	long
	enum  枚举定义
    union
	char
	float
	short
	unsigned
	signed
	void
	int
	double
	
	--变量定义
	const：const修饰的数据类型是指常类型，常类型的变量或对象的值是不能被更新的
	       好处：https://zhidao.baidu.com/question/96430567.html
	
	typedef：定义类型；和struct配合
	       具体：https://blog.csdn.net/superhoy/article/details/53504472
	
	struct：定义结构变量
	            struct string 
				 { 
					  char name[8]; 
					  int age; 
					  float wage1, wage2, wage3, wage4, wage5; 
				 }; 
				 struct string p1; 
	             struct string p2; 
				 p1.age =2
	             p2.wage1
				 https://blog.csdn.net/tuoguang/article/details/46928481
	
	sizeof ：指文件或者数据占的内存(字节) ！= strlen 指字符的长度
	        与strlen的区别：https://zhidao.baidu.com/question/12033577.html
	volatile：定义：A situation that is volatile is likely to change suddenly and unexpectedly.
	          编译器不会对此种变量进行优化消失
	          https://zhuanlan.zhihu.com/p/33074506
	
	_Packed：字节对齐
	
