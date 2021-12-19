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

