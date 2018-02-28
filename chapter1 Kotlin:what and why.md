```
本章涵盖：
  1.kotlin的一个基本代码示范
  2.Kotlin语言的主要特性
  3.Kotlin可应用于Android和服务端开发
  4.Kotlin区别于其他编程语言的方面
  5.Kotlin代码的书写和运行
 ```
 ### 1.1 Kotlin初探
 
   首先，Kotlin是什么？他是新的基于Java平台的编程语言。Kotlin具有简洁，安全，易用等特点，并且专注于和Java
 代码的互操作。他几乎能用于所有Java能被使用的地方，比如服务端开发，Android apps,等等。Kotlin在现有的Java
 包和Java框架下能很好的工作，并且和Java的执行水平一样。
 
 下面通过一个例子来示范一下Kotlin.这个例子定义了一个Person类，创建了一个people的集合，找出年龄最大的一个并且打印了出来；
 即便是这一小段代码，你也能看到很多Kotlin的特性。我们对一些代码加了高亮方便你在后面对照。对代码的解释有些简短，不过如果
 还是有一些不明白，不要担心，稍后我们将详细地讨论他们。
 如果你想运行这个示例，一个简便的做法是使用线上的环境，地址是[https://try.kotl.in](https://try.kotl.in).输入以下的例子
 并点击运行按钮，代码就能执行了。
 
 ```kotlin
 data class Person(val name:String,           1)
                   val age:Int?=null)         2)
fun main(args:Array<String>){
  val persons = listOf(Person("Alice"),
                       Person("Bob",age=29))
                       val oldest = persons.maxBy(it.age?:0)
                       println("The oldest is :$oldest")
}
 ```
