---
Java中的变量与常量
---  
> Java中的关键字  
- Java 关键字是区分大小写的哦！所以 void 是关键字，但 Void 就不是了~~  
- Java中的关键字：Java 语言中有一些具有特殊用途的词被称为关键字。  
- 常用关键字：abstract,boolean,break,byte,case,catch,char,class,  
  continue,default,do double,else,extends,false,final,finally,float,  
  for,if,implements,import,instanceof,int,interface,long,native,new,  
  null,package,private,protected,public,return,short,static,super,  
  switch,synchronized,this,throw,throws,transient,true,try,void,  
  volatile,while.  

> Java标识符  
- 标识符就是用于给 Java 程序中变量、类、方法等命名的符号。  
- 使用标识符时，需要遵守几条规则：  
  1. 标识符可以由字母、数字、下划线（_）、美元符（$）组成，但不能包含 @、%、空格等其它特殊字符，  
  不能以数字开头。譬如：123name 就是不合法滴  
  2.  标识符不能是 Java 关键字和保留字（ Java 预留的关键字，以后的升级版本中有可能作为关键字）  
  ，但可以包含关键字和保留字。如：不可以使用 void 作为标识符，但是 Myvoid 可以  
  3. 标识符是严格区分大小写的。 所以涅，一定要分清楚 imooc 和 IMooc 是两个不同的标识符哦！  
  4. 标识符的命名最好能反映出其作用，做到见名知意。  
  
> 变量  
- 在 Java 中，我们通过三个元素描述变量：变量类型、变量名以及变量值。  
  - 例如，我们定义了一个变量 love ，用来保存一个字符串 “imooc” , 在程序中只要找到了 love   
  这个变量，就能找到存储在里面的 ”imooc”！当然，我们也可以把 love 里面的值更换成新的字符串 “i love imooc” ！  

> 变量名命名规则  
1. 变量名由多单词组成时，第一个单词的首字母小写，其后单词的首字母大写，俗称骆驼式命名法（也称驼峰命名法），如 myAge  
2. 变量命名时，尽量简短且能清楚的表达变量的作用，做到见名知意。如：定义变量名 stuName 保存“学生姓名”信息  
3. Java 变量名的长度没有限制，但 Java 语言是区分大小写的，所以 price 和 Price 是两个完全不同的变量哦！  
- 多个字符串连接时用+连接，换行使用“\n”  

> Java中的数据类型  
- Java 语言是一种强类型语言。通俗点说就是，在 Java 中存储的数据都是有类型的，而且必须在编译时就确定其类型。  
- 数据类型：
  - 基本数据类型：1）数值型：整数（byte，short，int，long）浮点（float，double）  
  - 字符型（char）  
  - 布尔型（boolean）  
  - 引用数据类型：1）类（class）2）接口（interface）3）数组  
- float变量赋值时在数值后面添加字母f  float wight=60.1f;  
- char变量赋值时用单引号引起来 ‘A’ char level='A'  

> Java中变量的使用规则  
1. Java 中的变量需要先声明后使用.  
2. 变量使用时，可以声明变量的同时进行初始化,也可以先声明后赋值.  
3. 变量中每次只能赋一个值，但可以修改多次.  
4. main 方法中定义的变量必须先赋值，然后才能输出.  
5. 虽然语法中没有提示错误，但在实际开发中，变量名不建议使用中文，容易产生安全隐患，譬如后期跨平台操作时出现乱码等等.  
- 对于基本类型 用小写 如int char boolean float double  对于引用类型 用大写 如String  

> 自动类型转换  
- 在Java程序中，不同的基本数据类型之间京城需要进行相互转换。
- 自动转换需要满足的条件：  
  1. 目标类型能与源类型兼容，如double型兼容int型，但是char型不能兼容int型。  
  2. 目标类型大于源类型，如double型的长度为8字节，int类型为4字节，因此double类型的变量里直接可以存放int类型的数据，但反过来就不可以了。

> 强制类型转换  
- 语法：( 数据类型 ) 数值  
- 强制类型转换可能会造成数据的丢失哦  
  - double avg1 = 75.8;  
    int avg2 = (int)avg1;  //将double类型强制转换为int类型  
    
 > Java常量的应用  
 - 语法：final 常量名 = 值;  
 - 常量名一般使用大写字符  
 - 程序中使用常量可以提高代码的可维护性。  

> 如何在Java中使用注释  
- Java 中注释有三种类型：单行注释、多行注释、文档注释  
- 被注释的代码块在程序运行时是不会被执行的~~  
- 我们可以通过 javadoc 命令从文档注释中提取内容，生成程序的 API 帮助文档。  
- PS：使用文档注释时还可以使用 javadoc 标记，生成更详细的文档信息：  
       @author 标明开发该类模块的作者  
       
       @version 标明该类模块的版本  

       @see 参考转向，也就是相关主题  

       @param 对方法中某参数的说明  

       @return 对方法返回值的说明  

       @exception 对方法可能抛出的异常进行说明  
