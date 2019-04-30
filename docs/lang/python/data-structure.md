# 数据结构

## list

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
