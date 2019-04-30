# 计算机语言

## 语言的演进

## 语言的分类
根据计算机语言类型系统，可以对其进行分类：

### 编译型和解释型
语言在执行之前是否需要进行编译，通过编译器转换成中间态或者系统语言执行，这是编译型语言，最典型的编译型语言就是Java， Java语言在被执行前需要编译成JVM能读取的语言，然后通过JVM去执行。

如果不需要编译，语言在执行的时候需要一个解释器去将语言转换成机器能执行的语言，比如转换成汇编语言，这样机器就可以直接执行。最典型的解释型语言就是Python。

### 动态语言和静态语言
动态和静态的区分是根据语言的类型系统来区分的，当一个变量在初始化或者定义的时候，动态语言不做类型检查，允许其不强制指定类型，根据变量的赋值去自动判断类型，典型的动态语言有：Python, ruby, javascript等。

静态语言是需要在变量定义的时候需要明确指定类型，它会在编译期间检查类型，一旦发现类型与赋值不一致就会报错，典型的静态语言有：Java, C#, C, C++等。

### 强类型和弱类型
强类型是指一个变量定义类型之后就不能改变其类型，这样就会类型安全，而弱类型就是允许变量有不同类型，这样就会类型不安全，强类型语言有：python, java, C#等，弱类型语言有: vbscript等

# 参考
* [history of programming language](https://en.wikipedia.org/wiki/History_of_programming_languages)
* [programming language](https://en.wikipedia.org/wiki/Programming_language)