# java 语法糖

> 语法糖（Syntactic Sugar），也称糖衣语法，是由英国计算机学家 Peter.J.Landin 发明的一个术语，
指在计算机语言中添加的某种语法，这种语法对语言的功能并没有影响，但是更方便程序员使用。
Java 中最常用的语法糖主要有 

 * 泛型 
 * 自动装箱 
 * 自动拆箱
 * for-each循环
 * 变长参数
 * 内部类
 * 枚举类
 * 断言（assert）
 * ...

> 虚拟机并不支持这些语法，它们在编译阶段就被还原回了简单的基础语法结构，这个过程成为解语法糖。
 
> 泛型是 JDK1.5 之后引入的一项新特性，Java 语言在还没有出现泛型时，
只能通过 Object 是所有类型的父类和类型强制转换这两个特点的配合来实现泛型的功能，
这样实现的泛型功能要在程序运行期才能知道 Object 真正的对象类型，在 javac 编译期，
编译器无法检查这个 Object 的强制转型是否成功，这便将一些风险转接到了程序运行期中。
 
> Java 语言在 JDK1.5 之后引入的泛型实际上只在程序源码中存在，在编译后的字节码文件中，
就已经被替换为了原来的原生类型，并且在相应的地方插入了强制转型代码，因此对于运行期的Java语言来说，
ArrayList和 ArrayList就是同一个类。所以泛型技术实际上是 Java 语言的一颗语法糖，
Java 语言中的泛型实现方法称为类型擦除，基于这种方法实现的泛型被称为伪泛型。

> 想要分析java中的语法糖只需要研究反编译出的class文件即可。

## 1 java语法糖之泛型与类型擦除
## 2 java语法糖之自动拆装箱
## 3 java语法糖之for-each循环
## 4 java语法糖之可变参数
## 5 java语法糖之条件编译
## 6 java语法糖之内部类
## 7 java语法糖之断言语句
## 8 java语法糖之对枚举和字符串的switch支持
## 9 java语法糖之枚举类
## 10 java语法糖之带资源的try
