# README

## USAGE

Learn keywords such as:
- auto
- extern
- static
- register
- const
- volatile
- restricted
- \_Thread\_local
- \_Atomic

Learn functions like rand(), srand(), time(), malloc(), calloc() and free().

Learn how to estimate or make sure of the scope of a variable and its life cycle.

## Concepts

### 对象

> 我的理解：对象是运行过程中的实际存在。标识符是在代码中的存在。似乎这一区别很重要。

对象是一块被存储了特定数据的内存（不是 OOP 中的类对象）。

对象可存在与函数的执行期，也可以存在于它所在函数的执行期。对于并发编程，对象可以在特定线程的执行期存在。可以通过函数调用的方式显式分配内存和释放内存。



### 标识符

标识符是一个名称，用于指定特定对象上的内容。（那为什么要叫标识符，直接说名称可以用于指定对象上的内容不就好了？）

标识符可以用作用域和链接来描述。标识符的作用域和链接表明了程序的哪些部分可以使用它。

标识符可以在源代码的多文件中共享、可用于特定文件的任意函数中、可仅限于特定函数中使用，甚至只在函数中的某部分使用。


### 存储期

用于描述对象在内存中保留了多长时间。

### 链接



### 作用域

作用域描述程序中可访问标识符的区域。一个 C 变量的作用域可以是块作用域、函数作用域、函数原型作用域或者文件作用域。

- 块作用域：一对花括号括起来的代码区域。函数的形式参数也属于块作用域，这和最开始块作用域的变量必须声明在块的开头有关，但 C99 以后可以在块的任意位置声明变量。

- 函数作用域：函数作用域仅用于 goto 语句的标签（什么是 goto 语句，什么是标签？）


- 函数原型作用域：指函数原型的形参的定义到结束这一段。编译器只关注形参的类型。

- 文件作用域：如果变量的定义在函数的外面，则具有文件作用域。具有文件作用域的变量，从它的定义处到该定义所在文件的末尾均可见（可见是什么意思？可被调用？）

To be written...
