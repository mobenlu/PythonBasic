
### Task1

### 1. 环境搭建

**anaconda环境配置**

- Download and install Anaconda
https://www.anaconda.com/distribution/#download-section

- conda upgrade --all

- conda install/remove/upgrade/list/search package_name

**解释器**

- CPython
**当我们从Python官方网站下载并安装好Python 3.x后，我们就直接获得了一个官方版本的解释器：CPython。这个解释器是用C语言开发的，所以叫CPython。在命令行下运行python就是启动CPython解释器。CPython是使用最广的Python解释器。教程的所有代码也都在CPython下执行。**

- IPython
IPython是基于CPython之上的一个交互式解释器，也就是说，IPython只是在交互方式上有所增强，但是执行Python代码的功能和CPython是完全一样的。好比很多国产浏览器虽然外观不同，但内核其实都是调用了IE。CPython用>>>作为提示符，而IPython用In [序号]:作为提示符。

- PyPy
PyPy是另一个Python解释器，它的目标是执行速度。PyPy采用JIT技术，对Python代码进行动态编译（注意不是解释），所以可以显著提高Python代码的执行速度。绝大部分Python代码都可以在PyPy下运行，但是PyPy和CPython有一些是不同的，这就导致相同的Python代码在两种解释器下执行可能会有不同的结果。如果你的代码要放到PyPy下执行，就需要了解PyPy和CPython的不同点。

- Jython
Jython是运行在Java平台上的Python解释器，可以直接把Python代码编译成Java字节码执行。

- IronPython
IronPython和Jython类似，只不过IronPython是运行在微软.Net平台上的Python解释器，可以直接把Python代码编译成.Net的字节码。

### 2. python初体验
**print and input**
- Print


```python
print ("Hello World")
```

    Hello World


- input


```python
input ("Please input 'Hello World'")
```

    Please input 'Hello World'Hello World





    'Hello World'



3. python基础讲解

**python变量特性+命名规则**
- 变量名只能包含字母,数字和下划线,不能包含空格,不要将Python关键字和函数名用作变量名.

**注释方法**
- 单行注释以 # 开头
- 多行注释用三个单引号 ''' 或者三个双引号 """ 将注释括起来

**python中“：”作用**
- 用于定义分片、步长

**学会使用dir( )及和help( )**

**import使用**

**pep8介绍**



4. python数值基本知识
python中数值类型，int，float，bool，e记法等

算数运算符

逻辑运算符

成员运算符

身份运算符

运算符优先级
