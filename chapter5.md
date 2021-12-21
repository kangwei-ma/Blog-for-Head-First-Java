5 extra strength methods: flow control, operations and more

Chapter 5: Page 95-117
(PAGE 117-125 EXERCISES)

P95(124/719)   
 # 编写程序  
Operators, loops, generate random numbers, turn a string into an int.  

Learn it all by building something real.  
Simple version in this chapter and a complex version in chapter 6.  

P99  
	1. 找出类应该做的事情  
	2. 列出实例变量和方法  
	3. 编写方法的伪码  
	4. 编写方法的测试用程序  
	5. 实现类  
	6. 实现方法  
	7. 除错或重新设计  

伪码：专注于逻辑而不需要顾虑到程序语法，介于英语和java之间  
测试码：测试用的程序代码  
真实码：实际设计出的真正java程序代码  

P100  
伪码大致上包括三个部分：  
	1. 实例变量的声明  
	2. 方法的声明  
	3. 方法的逻辑  
	
	最重要的是方法的逻辑  
	因为他定义出会发生什么  
	这个部分会在稍后真正编写程序代码时，转译成如何发生    
例子 伪码 简单清晰的脉络  

P101  
写测试码，会让你更快更容易的写出程序代码。来自 XP极限编程方法论。   

XP极限编程方法论：    
	1. 多次经常性的小规模发布  
	2. 避免加入规格没有的功能  
	3. 先写测试用的程序  
	4. 正常工作上下班  
	5. 随时随地重构，也就是改善程序代码  
	6. 保持简单  
	7. 结伴进行工作，以便让大家清楚全局  
建议阅读专门的书籍，以免一知半解。  

P102  
编写测试码：  
如果checkYourself()方法已经写好的话，我要用什么样的测试码才能证明这个方法能够正确地运行？  

应该要测试的部分：  
	1. 对象的初始化  
	2. 赋值位置  
	3. 创建代表玩家猜设的字符串  
	4. 传入伪造的玩家猜测来调用checkYourself()方法  
	5. 列出结果以观察是否正确   

P104   真实码  
伪码让我们对于程序代码需要做什么有比较好的概念。  
	1. 取得玩家的猜测  
	2. 把用户猜测转换成int   
	3. 创建出保存返回结果的变量 以‘miss'作为默认值  
	4. 重复执行的循环  
	5. 比较格子与猜测值  
	6. 如果猜中， 递增命中数  
	7. 如果命中数为3， 返回击沉信息  （已经离开循环，但需要判断是否击沉）   
	8. 显示结果 返回给调用方  

P105   
一些细节  
每有会意，便欣然忘食！！！  
	1. 将string转换成int   
	Integer.parseInt("3")
	Integer是java内建类  
	parseInt是Integer的一个方法，能够将string解析  
	("3")采用string参数    
	 
	2. for循环  
	For(int cell: locationCells){}  
	把：读作in  也就是：
	For each int cells in location cells…  
	
	Int cell 声明出带有数组元素的变量。  
	在循环的每次循环中，  
	此变量的值都会带有不同的数组元素  
	直到跳出循环为止。  
	
	locationCells   要被逐个执行过的数组，  
	每循环一次，数组的下一个元素都赋给变量“cell”   
	
	3. 后递增操作符 post-increment  
	numOfHits++  
	++代表将其内值加一  
	意思是numOfHits = numOfHits +1  
	
	4. 中止指令  
	Break;  
	无条件立即跳出循环     
	
	
P107  
编写程序  
写出你的游戏伪码   
需要有下面的功能:  
	1. 创建出对象  
	2. 赋值给他  
	3. 要求玩家猜测  
	4. 检查猜测值  
	5. 重复猜测直到击沉为止  
	6. 显示玩家的猜测次数  
	
P109  
要点：  
	1. 你的java程序应该从高层的设计开始  
	2. 通常会在创建新的类时，写出下列3种东西：  
	伪码 测试码 真实码  
	3. 伪码应该描述要做什么事情而不是如何做  
	4. 使用伪码来帮助测试码的设计  
	5. 实现方法之前 应该要编写测试码  
	6. 如果知道要执行多少次，应该要使用for循环而不是while循环  
	7. 使用前置或后置的递增，为变量加一（比如x++）  
	8. 使用前置或后置的递减，为变量减一（比如x--）    
	9. 使用Integer.parseInt()来取得string的整数值     
	10. Integer.parseInt()只会在所给的string为数字时有作用  
	11. 使用break命令来提前跳出循环     


P111   
 ## 产生随机数   
Int randomNum = (int) (Math.random()*5)  

Int randomNum 声明一个表示随机数的变量  
(int) 这是一种类型转换（cast）他会强制编译器以所设定的类型进行处理。  
因为Math.random会返回double类型，  
而我们需要0-4之间的integer，  
因此需要将它转换成int    

Math是java内建的类  
random是math这个类内含的一个方法  
Math.random会返回一个0到1之间的数，  
所以*5会生出介于0-4之间的整数。  

 ## 取得玩家输入    
String guess = helper.getUserInput("enter a number");    

String guess 声明出这个变量来保存玩家输入的猜测值    
helper这是辅助性类的一个实例，它来自于我们还没有讨论到的GameHelper  
getUserInput这是GameHelper的一个方法，他会在印出提示字符串后等待玩家输入  
("enter a number")这个方法会以string参数当做提示来要求玩家，输入一个猜测的数字。  


P114  
For loop    
For(int i=0; i<100; i++){}    
	1. 初始化。创建变量i并赋值为0  
	2. Boolean测试：只要i小于100就重复执行  
	3. 重复表达式：在每趟重复过程的最后把i加1


P115  
 ### 前置和后置的区别：  
放在变量前面代表先执行加减操作  
然后再来运用变量的值  

 ### 比较for loop 和while loop：  

while循环只有boolean测试，  
他没有内建的初始化或者重复表达式。  
while适合用在不知道要循环几次的时候。  
while必须得声明并初始化-计数器变量  
在循环内将计数器递增    


P116  
 ###加强版的 for loop   
For(string name: nameArray){}   
String-数组元素的类型必须 与循环变量的类型匹配  
Name-声明会带有数组单一元素的循环变量；  
此变量在循环过程中会带有不同元素的值  
：代表in  
nameArray要被逐个运行的集合   
{}重复执行的部分放在这里  

在编译器眼中：  
	1. 创建名称为name的string变量  
	2. 将nameArray的第一个元素值赋给name  
	3. 执行重复的内容  
	4. 赋值给下一个元素name  
	5. 重复执行至所有元素都被运行为止。
![image](https://user-images.githubusercontent.com/88927644/146927918-0b83a41e-f5b5-4512-a201-11dd086a45c7.png)
