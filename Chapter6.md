6-java API 函数库  
 # 6 认识java的API  P125-165   
使用java函数库  
java内置有数百个类  
从函数库中找所需的功能就不用重复发明轮子了   

P132  
ArrayList 是java函数库中的另一个类  

P135  
arrayList 可以删除引用（元素），还可以动态地改变我的大小  
在运用primitive主数据类型的时候，数组会比arrayList快。  

P136  
 # arrayList与一般数组(array)的比较    
 ## arrayList     
在使用arrayList时，你只是在运用arrayList类型的对象，  
因此就跟运用其他的对象一样，  
你会使用“.”运算符来调用他的方法。   
 ## 一般数组
使用数组时，你会以特殊的数组语法来操作。    
这样的语法只能用在数组上  
虽然说数组也是对象   
但是他有自己的规则  
你无法调用它的方法  
最多只能存取他的length实例变量    

P137  
 # arrayList与一般数组array的比较   
	1. 一般数组在创建时就必须确定大小  
	但对于arrayList来说，你只需要创建出此类型的对象。  
	他不需要指定大小，  
	因为他会在加入或删除元素时，  
	自动地调整大小。  
	New string[2] 指定大小    
	New arrayList<String>()不需要指定大小  
	
	2. 存放对象给一般数组时，必须指定位置。  
	（介于0到比length小1之间的数字）  
	myList[1] = b;  指定索引值    
	如果索引值超越了数组的限制，就会报错。  
	
	使用arrayList时，  
	你可以用add(int, object)这个形式的方法，  
	来指定索引值，  
	或者使用add(object)的形式来让他自行管理大小。  
	myList.add(b);  不需要指定索引值  
	
	3. 一般数组使用特殊的语法  
arrayList是个普通对象，  
所以不会有特殊的语法。   
myList[1] 方括号是只用在数组(array)上的特殊语法。  

	4. 在java5.0中的arrayList是参数化的（parameterized）   
虽然arrayList不像一般数组有特殊的语法，  
但是他们在java5.0中有比较特殊的东西：  
参数化模型。  

arrayList<string>  
这里的string是类型参数。  
这代表string的集合，  
就像arrayList<dog>代表dog的集合。  




![image](https://user-images.githubusercontent.com/88927644/147094932-12684eae-5888-4884-a7a0-62dee0371e89.png)
