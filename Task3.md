
### 1、dict字典
- 定义
- 创建
- 字典的方法


```python
dic1={'name':'abc','sex':'male','professional':'Math'}
dic2={'name':'cdf','sex':'female','professional':'Eng'}
print(dic1['sex']);
dic1['child'] = ('1');
print(dic1['child']);
print (dic1)
print (dic2)
del dic1['name']
print (dic1)
dic =[dic1, dic2]
print(dic)
```

    male
    1
    {'name': 'abc', 'sex': 'male', 'professional': 'Math', 'child': '1'}
    {'name': 'cdf', 'sex': 'female', 'professional': 'Eng'}
    {'sex': 'male', 'professional': 'Math', 'child': '1'}
    [{'sex': 'male', 'professional': 'Math', 'child': '1'}, {'name': 'cdf', 'sex': 'female', 'professional': 'Eng'}]


### 2、 集合
- [Ref](http://www.runoob.com/python3/python3-set.html)
- 特性
- 创建
- 方法


```python
name = {'a','b','c','d','e'}
print(name)
name.add('f')
print(name)
l = len (name)
print(l)
```

    {'a', 'b', 'c', 'd', 'e'}
    {'a', 'b', 'c', 'd', 'e', 'f'}
    6


### 3、 判断语句（要求掌握多条件判断）


### 4、三目表达式



```python
h = 3 if 4>3 else 5
print(h)
```

    3


### 5、 循环语句


```python
for letter in 'Python':
    print (letter)

i=1
for i in range (1,5):
    print (i)
```

    P
    y
    t
    h
    o
    n
    1
    2
    3
    4

