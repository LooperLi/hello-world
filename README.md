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
	
三：数据类型
    1）基本类型：整数类型和浮点类型
	2）枚举类型
	3）void类型
	4）派生类型：指针，数组，结构类型，共用体类型和函数类型
	
	1：整数类型
		类型                存储大小                   值范围
		char                1 字节                     -128 到 127 或 0 到 255
		unsigned char       1 字节                     0 到 255
		signed char         1 字节                     -128 到 127
		int                 2 或 4 字节                -32,768 到 32,767 或 -2,147,483,648 到 2,147,483,647
		unsigned int        2 或 4 字节                0 到 65,535 或 0 到 4,294,967,295
		short               2 字节                     -32,768 到 32,767
		unsigned short      2 字节                     0 到 65,535
		long                4 字节                     -2,147,483,648 到 2,147,483,647
		unsigned long       4 字节                     0 到 4,294,967,295
		
		 a，默认为10进制 ，10 ，20。 
		 b，以0开头为8进制，045，021。 
		 c，以0b开头为2进制，0b11101101。 
		 d，以0x开头为16进制，0x21458adf。

    2:浮点类型
		类型                存储大小                   值范围                      精度
		float               4 字节                     1.2E-38 到 3.4E+38          6 位小数
        double              8 字节                     2.3E-308 到 1.7E+308        15 位小数
        long double         16 字节                    3.4E-4932 到 1.1E+4932      19 位小数

		单精度常量：2.3f 。
        双精度常量：2.3，默认为双精度
		
		
    3：void类型
		1-函数返回为空
             C 中有各种函数都不返回值，或者您可以说它们返回空。不返回值的函数的返回类型为空。例如 void exit (int status);
        2-函数参数为空
             C 中有各种函数不接受任何参数。不带参数的函数可以接受一个 void。例如 int rand(void);
	    3-指针指向 void
		     类型为 void * 的指针代表对象的地址，而不是类型。
			 例如，内存分配函数 void *malloc( size_t size );返回指向 void 的指针，可以转换为任何数据类型。
			 
			 
			 
四：变量
    1）最基本的变量
		char
		int
		float 1 8 23
		double 1 11 52
	
	2)变量的声明
		extern int i; //声明，不是定义
		int i;        //声明，也是定义
		
		打印  float--》%f  
		      double--》%lf
	3）左值和右值
	   左值可以被赋值，右值不可以
	   
	   
	   
五：常量
    1）整数常量
		0x 或 0X 表示十六进制，0 表示八进制，不带前缀则默认表示十进制。
		整数常量也可以带一个后缀，后缀是 U 和 L 的组合，
		U 表示无符号整数（unsigned），
		L 表示长整数（long）。
		后缀可以是大写，也可以是小写，U 和 L 的顺序任意。
	   
	2）浮点常量
		当使用小数形式表示时，必须包含整数部分、小数部分，或同时包含两者。
		当使用指数形式表示时， 必须包含小数点、指数，或同时包含两者。带符号的指数是用 e 或 E 引入的。？？？？？？
		3.14159       /* 合法的 */
		314159E-5L    /* 合法的 */
		510E          /* 非法的：不完整的指数 */
		210f          /* 非法的：没有小数或指数 */
		.e55          /* 非法的：缺少整数或分数 */

    3）字符常量
		转义序列         含义
        \\				\ 字符
		\'				' 字符
		\"				" 字符
		\?				? 字符
		\a				警报铃声
		\b				退格键
		\f				换页符
		\n				换行符
		\r				回车
		\t				水平制表符
		\v				垂直制表符
		\ooo			一到三位的八进制数
		\xhh . . .		一个或多个数字的十六进制数
		
	4）字符串常量
		字符串字面值或常量是括在双引号 "" 中的。
		
	5）定义常量
	   1-#define 预处理器  宏
       2-const 关键字
	   
六：存储类
	1）auto 存储类：所有局部变量默认的存储类。
	
	2）register 存储类：定义存储在寄存器中而不是 RAM 中的局部变量。
	                    这意味着变量的最大尺寸等于寄存器的大小（通常是一个词），且不能对它应用一元的 '&' 运算符（因为它没有内存位置）。
	
	3）static 存储类：全局变量的默认存储类
					  修饰局部变量可以在函数调用之间保持局部变量的值
					  
	4）extern 存储类：用来在另一个文件中声明一个全局变量或函数
	
	
	
七：运算符
    1）算术运算符
		+ - * / % ++ --
		
		a++和++a的区别
		a = 10 ;c = a++;这时a=11，c=10；
		a = 10 ;c = ++a;这时a=11，c=11；
		

	2）关系运算符
		==  !=  >  <  >=  <=
		
	3）逻辑运算符
		&&  ||  !
		
	4）位运算符
		&   |   ^  ~  <<  >>
		
		^ :如果存在于其中一个操作数中但不同时存在于两个操作数中，二进制异或运算符复制一位到结果中。
		~ ：取反
		
				利用异或 ^ 来交换两个数的值，而且不引入其他变量。
				unsigned int a=60;  //0011 1100
				unsigned int b=13;  //0000 1101
				a=a^b;              //a=a^b=0011 0001
				b=a^b;              //b=a^b=0011 1100  相当于b1=(a^b)^b
				a=a^b;              //a=a^b=0000 1101  相当于a1=(a^b)^((a^b)^b)
				
				
	5）赋值运算符
		=  +=  -=  *= 。。。。。。
		
	6）杂项运算符
	   sizeof（） ：计算变量内存的大小
	   &          ：取地址
	   *          ：指向一个变量
	   ？：       ：a=（b=10）?1:0;  b=10的时候a=1,否则a=0
	   
	7）运算符的优先级：http://www.runoob.com/cprogramming/c-operators.html

	
八：判断
	1）C 语言把任何非零和非空的值假定为 true，把零或 null 假定为 false。
		1：if else
		2：switch case


































	
