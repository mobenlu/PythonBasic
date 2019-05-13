
### Task2

**列表**
- 标志
- 基本操作(创建，append(),pop(),del(),拷贝)
- 列表相关方法
- https://www.runoob.com/python/python-lists.html


```python
list1 = ["a", "b", "c", "d"]
print('List1',list1)
print(list1[0])
list1.append('f')
print('List1',list1)
```

    List1 ['a', 'b', 'c', 'd']
    a
    List1 ['a', 'b', 'c', 'd', 'f']


**元组**
- 标志

Python的元组与列表类似，不同之处在于元组的元素不能修改。

元组使用小括号，列表使用方括号。

元组创建很简单，只需要在括号中添加元素，并使用逗号隔开即可。
- 基本操作(创建及不可变性)


```python
list1 = ("a", "b", "c", "d")
print('List1',list1)
print(list1[0])
```

    List1 ('a', 'b', 'c', 'd')
    a


**string字符串**
- 定义及基本操作(+，*，读取方式)

- 字符串相关方法
- https://www.runoob.com/python/python-strings.html


```python
String1 = 'Hello'
String2 = "world"
print (String1+String2)
print (String1[1]+String2[4])
print (String1*30)
print (String1[1:3]+String2[2:4])
print (("My name is %s and weight is %d kg!") % ('Zara', 21))
```

    Helloworld
    ed
    HelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHelloHello
    elrl
    My name is Zara and weight is 21 kg!


**字符串格式化问题**
- https://www.runoob.com/python/python-strings.html


```python
print (("My name is %s and weight is %d kg!") % ('Zara', 21))
```

    My name is Zara and weight is 21 kg!

