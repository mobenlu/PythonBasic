
### 1、函数关键字


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



```python
4.函数返回值

```

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

