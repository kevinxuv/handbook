# Python

python是一门解释性语言，弱类型，动态语言，我们可以先看看Python能做什么 [fullstackpython](https://www.fullstackpython.com/table-of-contents.html)

## 优点

Python显著的优点是语法简洁和类自然语言，这有助于提高开发代码的效率，提高开发者的生产力，而且还提供很多编程能力：

### 函数式编程(functional programming)

### 元编程(meta programming)

### 面向对象编程(oop)

### 结构化编程(structured programming)

## 缺点

### 语法灵活

Python代码的执行完全依赖解释器的性能，而且由于Python的灵活性，完全可以写出一些奇奇怪怪的代码，带来的问题除了维护成本上的考虑以外，还有就是降低了Python代码的运行速度，Python的解释器本身就很低效，Python给开发者带来友好的开发体验的同时也给Python解释器带来很多负担

### 动态类型

动态特性带来的问题就是在IDE支持这块，没有静态语言支持的好，在编译时无法做类型检查。

### GIL

由于GIL的限制，导致Python就是一个单线程语言，无法通过多线程去利用多核，只能通过多进程来利用多核，但是又带来了多进程管理的问题，天生性能比不上Java这种多线程语言，而且在网络I/O方面又有netty这么优秀的NIO框架实现。

### 性能

Python语言的性能问题是其比较明显的问题，在某些业务场景这个问题并不突出，但是在某些对程序性能要求比较高的业务场景，这个问题就比较突出，尤其是当前盛行微服务，服务拆分越来越多，服务的性能会受到很多方面的影响，磁盘I/O，网络I/O，单个实例的并发等。

## 数据类型

### list

当你需要复制一个list的时候，用赋值的方法赋值给另外一变量，只会把引用指向新的变量，实际指向的内存地址是一样的，当你改变其值的时候，2个变量都会改变：

```
$ a = [1,2,3]
$ b = a
$ a.remove(2)
$ print a, b
$ [1,3] [1,3]
$ print a==b
$ true
```
有几种方法复制一个list，可参考[How to clone or copy a list?](https://stackoverflow.com/questions/2612802/how-to-clone-or-copy-a-list)

## 参考

* [wikipedia](https://en.wikipedia.org/wiki/Python_\(programming_language\))