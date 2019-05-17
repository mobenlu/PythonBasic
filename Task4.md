
### 1、函数关键字

在定义 Python 函数时可定义形参（形式参数的意思），这些形参的值要等到调用时才能确定下来，由函数的调用者负责为形参传入参数值。简单来说，就是谁调用函数，谁负责传入参数值。

Python 函数的参数名不是无意义的，Python 允许在调用函数时通过名字来传入参数值。因此，Python 函数的参数名应该具有更好的语义，这样程序可以立刻明确传入函数的每个参数的含义。

按照形参位置传入的参数被称为位置参数。如果使用位置参数的方式来传入参数值，则必须严格按照走义函数时指定的顺序来传入参数值；如果根据参数名来传入参数值，则无须遵守定义形参的顺序，这种方式被称为关键字（keyword）参数。


```python
# 定义一个函数
def girth(width , height):
    print("width: ", width)
    print("height: ", height)
    return 2 * (width + height)

print("传统调用函数的方式，根据位置传入参数")
print(girth(3.5, 4.8))

print("根据关键字参数来传入参数")
print(girth(width = 3.5, height = 4.8))

print("使用关键字参数时可交换位置")
print(girth(height = 4.8, width = 3.5))

print("部分使用关键字参数，部分使用位置参数")
print(girth(3.5, height = 4.8))
```

    传统调用函数的方式，根据位置传入参数
    width:  3.5
    height:  4.8
    16.6
    根据关键字参数来传入参数
    width:  3.5
    height:  4.8
    16.6
    使用关键字参数时可交换位置
    width:  3.5
    height:  4.8
    16.6
    部分使用关键字参数，部分使用位置参数
    width:  3.5
    height:  4.8
    16.6


### 2、函数的定义
[REF](https://www.runoob.com/python/python-functions.html)



```python
# 定义函数
def printme( str ):
   "打印任何传入的字符串"
   print (str);
   return;
 
# 调用函数
printme("我要调用用户自定义函数!");
printme("再次调用同一函数");
```

    我要调用用户自定义函数!
    再次调用同一函数


### 3、函数参数与作用域
[REF1](https://www.jianshu.com/p/2f3dc7900d95?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation)

- 不可变参数”通过值”进行传递。像整数和字符串这样的对象是通过对象引用而不是拷贝进行的，但是因为不论怎么样都不可能在原处改变不可变对象，实际的效果就很像创建了一份拷贝。

- 可变对象是通过”指针”进行传递的。这就意味着，可变对象能够在函数内部进行原处修改。

### 4、函数返回值
[REF1](https://www.jianshu.com/p/2f3dc7900d95?utm_campaign=maleskine&utm_content=note&utm_medium=seo_notes&utm_source=recommendation)

### 5、File
[REF](https://www.runoob.com/python/file-methods.html)

- 打开文件方式（读写两种方式）

open(file, mode='r', buffering=-1, encoding=None, errors=None, newline=None, closefd=True, opener=None)
注意：使用 open() 方法一定要保证关闭文件对象，即调用 close() 方法。

https://blog.csdn.net/zhengxiangwen/article/details/55148287


- 文件对象的操作方法
- 学习对Excel及CSV文件进行操作



```python
# -*- coding: utf-8 -*-
import os
file1 = r'/Users/mojinteng/Documents/GitHub/PythonBasic/001.txt'
#1#
f = open(file1)               # 返回一个文件对象 
line = f.readline()               # 调用文件的 readline()方法 
while line: 
    print(line, end = ''),# 在 Python 3 中使用 
    line = f.readline() 
f.close()
```

    I love programming.


```python
#2
# -*- coding: utf-8 -*-
import os
file1 = r'/Users/mojinteng/Documents/GitHub/PythonBasic/001.txt'
for line in open(file1): 
    print (line)

```

    I love programming.



```python
# -*- coding: utf-8 -*-
import os
file1 = r'/Users/mojinteng/Documents/GitHub/PythonBasic/001.txt'
#3
f = open(file1) 
lines = f.readlines()    #读取全部内容 ，并以列表方式返回
    
with open(file1, 'w') as file1:
    file1.write('I love programming.')
for line in lines: 
    print (line)
```

    I love programming.


### 6、Os模块
[操作系统接口模块](https://docs.python.org/zh-cn/3.7/library/os.html)


### 7、Datetime模块
[基础日期/时间数据类型](https://docs.python.org/zh-cn/3.7/library/datetime.html?highlight=datetime#module-datetime)

[Python 日期和时间](https://www.runoob.com/python/python-date-time.html)


```python
import time
 
localtime = time.localtime(time.time())
print ("Shanghai is #", localtime)
localtime = time.asctime( time.localtime(time.time()))
print ("Shanghai is #", localtime)

localtime2 = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
print ("Shanghai is #", localtime2)

localtime3 = time.strftime("%a %b %d %H:%M:%S %Y", time.localtime())
print ("Shanghai is #", localtime3)

```

    Shanghai is # time.struct_time(tm_year=2019, tm_mon=5, tm_mday=17, tm_hour=8, tm_min=13, tm_sec=14, tm_wday=4, tm_yday=137, tm_isdst=0)
    Shanghai is # Fri May 17 08:13:14 2019
    Shanghai is # 2019-05-17 08:13:14
    Shanghai is # Fri May 17 08:13:14 2019

