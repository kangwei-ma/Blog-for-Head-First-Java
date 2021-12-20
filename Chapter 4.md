 # Chapter 4 Methods use instance variables  
 ## How objects behave （方法操作实例变量）  

P71  
对象有状态和行为：  
	• 状态：实例变量  
	• 行为：方法  
二者之间有何关联？  
e.g. 体重大的狗叫声大  
这就是面向对象的重点  
行为会依据状态来决定  

记住：类所描述的对象知道什么 执行什么  
在编写类时， 你是在描述java虚拟机  
应该如何制作该类型的对象  
同一类的每个实例都带有相同的方法  
但方法可以根据实例变量的值  
来表现不同的行为  

P73  
dog这个类有个称为size的实例变量，  
bark()会用他来决定使用哪一种声音。  

P74   
 ## 方法的参数  

argument 实参  
Parameter 形参  

A method uses parameters.   
A caller passes arguments.

Arguments are the things you pass into the methods. 
A parameter is nothing more than a local variable.  

If a method takes a parameter, you must pass it something.  
(must be the value of appropriate type)  


P75  
方法可以有返回值，但目前都是void，代表没有返回任何东西。

P76  
可以有多个参数。  
声明的时候用逗号分开  
传入的时候也是用逗号分开  
最重要的是：  
如果方法有参数  
一定要以正确的数量、类型、和顺序   
来传递参数。  

可以将变量当做参数传入，只要类型相符  

P77

java是通过值传递的，  
也就是说通过拷贝传递  
方法无法改变 调用方所传入的参数  

P78  
参数和返回值  
java中所传递的所有东西都是值。  
变量所携带的值  

方法只能声明单一的返回值  
java注重类型  

 # 要点  
类定义对象所知及所为  
对象所知者 是实例变量  
对象所为者 是方法  
方法可依据实例变量来展现不同的行为  

方法可使用参数，可以传入一个或多个值给方法  
传给方法的参数必须符合  声明时的数量 顺序和类型。  
传入与传出的方法的值的类型  可以隐含的放大或是明确的缩小  

传给方法的参数值可以是：  
	1. 直接指定的文字或数字  
	2. 与所声明参数相同类型的变量    

方法必须声明返回类型  
void类型代表方法不返回任何东西  

如果方法声明了 非void的返回类型  
那就一定要返回 与声明类型相同的值。  



P79  
 ### 运用-参数与返回类型  
Getter and setter （更符合java命名习惯）  
正式：Accessor and mutator  
Getter: 返回实例变量的值  
setter：取用一个参数来设定实例变量的值  

P80   
 #  封装 encapsulation  
必须通过setter来设定变量而不是直接的存取。  

P80  
封装的基本原则（维持安全性）：  
将实例变量标记为private；  
将getters & setters标记为public （来控制存取动作）。  

P81  
强迫其他程序一定得经过setter，  
如此setter就能够检查参数并判断是否可以执行。  
可以退回不合理的值。  

P83  
 ##  数组中对象的行为   
How do objects in an array behave?   
Just like any other object   
The only difference is how you get to them  
In other words, how you get the remote control  


P84  
实例变量永远都会有默认值。  
如果你没有明确的赋值给实例变量，  
或者没有调用setter，    
实例变量还是会有值。  

P85  
 ##  实例变量与局部变量之间的差别  
	1. 实例变量是声明在类中 而不是在方法中    
	2. 局部变量是声明在方法中的。  
	3. 局部变量在使用前必须初始化     
	
局部变量没有默认值！
如果在变量被初始化前就要使用的话，  
编译器会显示错误。  

那方法的参数呢？  
局部变量的规则也适用于他们身上吗？  
方法的参数基本上与局部变量是相同的  
他们都是在方法中声明的   
但参数并没有未声明的问题  
所以编译器也不可能对这种事情显示出错误  

因为如果调用方法而没有赋值参数  
编译器就会显示错误。  
所以说参数一定会被初始化  
编译器会确保方法被调用时，  
有与声明相符的参数    
且参数会自动地被赋值进去。  

P86  
 ## 变量的比较（primitive主数据类型或引用）    
使用==来比对primitive主数据类型，  
或者判断两个引用是否引用同一个对象  
使用equals()来判断两个对象是否在意义上相等    

P87  
Passing by value is passing by copy  



