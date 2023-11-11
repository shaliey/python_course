# 实验六 Python函数

班级： 21计科4班

学号： B20210302426

姓名： 陈佩儿

Github地址：<https://github.com/shaliey/python_course>

CodeWars地址：<https://www.codewars.com/users/shaliey>


## 实验目的

1. 学习Python函数的基本用法
2. 学习lambda函数和高阶函数的使用
3. 掌握函数式编程的概念和实践

## 实验环境

1. Git
2. Python 3.10
3. VSCode
4. VSCode插件

## 实验内容和步骤

### 第一部分

Python函数

完成教材《Python编程从入门到实践》下列章节的练习：

- 第8章 函数

---

### 第二部分

在[Codewars网站](https://www.codewars.com)注册账号，完成下列Kata挑战：

---

#### 第一题：编码聚会1

难度： 7kyu

你将得到一个字典数组，代表关于首次报名参加你所组织的编码聚会的开发者的数据。
你的任务是返回来自欧洲的JavaScript开发者的数量。
例如，给定以下列表：

```python
lst1 = [
  { 'firstName': 'Noah', 'lastName': 'M.', 'country': 'Switzerland', 'continent': 'Europe', 'age': 19, 'language': 'JavaScript' },
  { 'firstName': 'Maia', 'lastName': 'S.', 'country': 'Tahiti', 'continent': 'Oceania', 'age': 28, 'language': 'JavaScript' },
  { 'firstName': 'Shufen', 'lastName': 'L.', 'country': 'Taiwan', 'continent': 'Asia', 'age': 35, 'language': 'HTML' },
  { 'firstName': 'Sumayah', 'lastName': 'M.', 'country': 'Tajikistan', 'continent': 'Asia', 'age': 30, 'language': 'CSS' }
]
```

你的函数应该返回数字1。
如果，没有来自欧洲的JavaScript开发人员，那么你的函数应该返回0。

注意：
字符串的格式将总是"Europe"和"JavaScript"。
所有的数据将始终是有效的和统一的，如上面的例子。

这个卡塔是Coding Meetup系列的一部分，其中包括一些简短易行的卡塔，这些卡塔是为了让人们掌握高阶函数的使用。在Python中，这些方法包括：`filter`, `map`, `reduce`。当然也可以采用其他方法来解决这些卡塔。

[代码提交地址](https://www.codewars.com/kata/coding-meetup-number-1-higher-order-functions-series-count-the-number-of-javascript-developers-coming-from-europe)

---

#### 第二题： 使用函数进行计算

难度：5kyu

这次我们想用函数来写计算，并得到结果。让我们看一下一些例子：

```python
seven(times(five())) # must return 35
four(plus(nine())) # must return 13
eight(minus(three())) # must return 5
six(divided_by(two())) # must return 3
```

要求：

- 从0（"零"）到9（"九"）的每个数字都必须有一个函数。
- 必须有一个函数用于以下数学运算：加、减、乘、除。
- 每个计算都由一个操作和两个数字组成。
- 最外面的函数代表左边的操作数，最里面的函数代表右边的操作数。
- 除法应该是整数除法。

例如，下面的计算应该返回2，而不是2.666666...。

```python
eight(divided_by(three()))
```

代码提交地址：
<https://www.codewars.com/kata/525f3eda17c7cd9f9e000b39>

---

#### 第三题： 缩短数值的过滤器(Number Shortening Filter)

难度：6kyu

在这个kata中，我们将创建一个函数，它返回另一个缩短长数字的函数。给定一个初始值数组替换给定基数的 X 次方。如果返回函数的输入不是数字字符串，则应将输入本身作为字符串返回。

例子：

```python
filter1 = shorten_number(['','k','m'],1000)
filter1('234324') == '234k'
filter1('98234324') == '98m'
filter1([1,2,3]) == '[1,2,3]'
filter2 = shorten_number(['B','KB','MB','GB'],1024)
filter2('32') == '32B'
filter2('2100') == '2KB';
filter2('pippi') == 'pippi'
```

代码提交地址：
<https://www.codewars.com/kata/56b4af8ac6167012ec00006f>

---

#### 第四题： 编码聚会7

难度： 6kyu

您将获得一个对象序列，表示已注册参加您组织的下一个编程聚会的开发人员的数据。

您的任务是返回一个序列，其中包括最年长的开发人员。如果有多个开发人员年龄相同，则将他们按照在原始输入数组中出现的顺序列出。

例如，给定以下输入数组：
```python
list1 = [
  { 'firstName': 'Gabriel', 'lastName': 'X.', 'country': 'Monaco', 'continent': 'Europe', 'age': 49, 'language': 'PHP' },
  { 'firstName': 'Odval', 'lastName': 'F.', 'country': 'Mongolia', 'continent': 'Asia', 'age': 38, 'language': 'Python' },
  { 'firstName': 'Emilija', 'lastName': 'S.', 'country': 'Lithuania', 'continent': 'Europe', 'age': 19, 'language': 'Python' },
  { 'firstName': 'Sou', 'lastName': 'B.', 'country': 'Japan', 'continent': 'Asia', 'age': 49, 'language': 'PHP' },
]
```

您的程序应该返回如下结果：

```python
[
  { 'firstName': 'Gabriel', 'lastName': 'X.', 'country': 'Monaco', 'continent': 'Europe', 'age': 49, 'language': 'PHP' },
  { 'firstName': 'Sou', 'lastName': 'B.', 'country': 'Japan', 'continent': 'Asia', 'age': 49, 'language': 'PHP' },
]
```

注意：

- 输入的列表永远都包含像示例中一样有效的正确格式的数据，而且永远不会为空。

代码提交地址：
<https://www.codewars.com/kata/582887f7d04efdaae3000090>

---

#### 第五题： Currying versus partial application

难度： 4kyu

[Currying versus partial application](https://2ality.com/2011/09/currying-vs-part-eval.html)是将一个函数转换为具有更小arity(参数更少)的另一个函数的两种方法。虽然它们经常被混淆，但它们的工作方式是不同的。目标是学会区分它们。

Currying

是一种将接受多个参数的函数转换为以每个参数都只接受一个参数的一系列函数链的技术。

Currying接受一个函数：

```python
f：X × Y → R
```

并将其转换为一个函数：

```python
f'：X → (Y → R)
```

我们不再使用两个参数调用f，而是使用第一个参数调用f'。结果是一个函数，然后我们使用第二个参数调用该函数来产生结果。因此，如果非curried f被调用为：

```python
f(3, 5)
```

那么curried f'被调用为：

```python
f'(3)(5)
```

示例
给定以下函数：

```python
def add(x, y, z):
  return x + y + z
```

我们可以以普通方式调用：

```python
add(1, 2, 3) # => 6
```

但我们可以创建一个curried版本的add(a, b, c)函数：

```python
curriedAdd = lambda a: (lambda b: (lambda c: add(a,b,c)))
curriedAdd(1)(2)(3) # => 6
```

Partial application
是将一定数量的参数固定到函数中，从而产生另一个更小arity(参数更少)的函数的过程。

部分应用接受一个函数：

```python
f：X × Y → R
```

和一个固定值x作为第一个参数，以产生一个新的函数

```python
f'：Y → R
```

f'与f执行的操作相同，但只需要填写第二个参数，这就是其arity比f的arity少一个的原因。可以说第一个参数绑定到x。

示例:

```python
partialAdd = lambda a: (lambda *args: add(a,*args))
partialAdd(1)(2, 3) # => 6
```

你的任务是实现一个名为curryPartial()的通用函数，可以进行currying或部分应用。

例如：

```python
curriedAdd = curryPartial(add)
curriedAdd(1)(2)(3) # => 6

partialAdd = curryPartial(add, 1)
partialAdd(2, 3) # => 6
```

我们希望函数保持灵活性。

所有下面这些例子都应该产生相同的结果：

```python
curryPartial(add)(1)(2)(3) # =>6 
curryPartial(add, 1)(2)(3) # =>6 
curryPartial(add, 1)(2, 3) # =>6 
curryPartial(add, 1, 2)(3) # =>6 
curryPartial(add, 1, 2, 3) # =>6 
curryPartial(add)(1, 2, 3) # =>6 
curryPartial(add)(1, 2)(3) # =>6 
curryPartial(add)()(1, 2, 3) # =>6 
curryPartial(add)()(1)()()(2)(3) # =>6 

curryPartial(add)()(1)()()(2)(3, 4, 5, 6) # =>6 
curryPartial(add, 1)(2, 3, 4, 5) # =>6 

curryPartial(curryPartial(curryPartial(add, 1), 2), 3) # =>6
curryPartial(curryPartial(add, 1, 2), 3) # =>6
curryPartial(curryPartial(add, 1), 2, 3) # =>6
curryPartial(curryPartial(add, 1), 2)(3) # =>6
curryPartial(curryPartial(add, 1)(2), 3) # =>6
curryPartial(curryPartial(curryPartial(add, 1)), 2, 3) # =>6
```

代码提交地址：
<https://www.codewars.com/kata/53cf7e37e9876c35a60002c9>

---

### 第三部分

使用Mermaid绘制程序流程图

安装VSCode插件：

- Markdown Preview Mermaid Support
- Mermaid Markdown Syntax Highlighting

使用Markdown语法绘制你的程序绘制程序流程图（至少一个），Markdown代码如下：

![程序流程图](/Experiments/img/2023-08-05-22-00-00.png)

显示效果如下：

```mermaid
flowchart LR
    A[Start] --> B{Is it?}
    B -->|Yes| C[OK]
    C --> D[Rethink]
    D --> B
    B ---->|No| E[End]
```

查看Mermaid流程图语法-->[点击这里](https://mermaid.js.org/syntax/flowchart.html)

使用Markdown编辑器（例如VScode）编写本次实验的实验报告，包括[实验过程与结果](#实验过程与结果)、[实验考查](#实验考查)和[实验总结](#实验总结)，并将其导出为 **PDF格式** 来提交。

## 实验过程与结果

请将实验过程与结果放在这里，包括：

- [第一部分 Python函数](#第一部分)
- [第二部分 Codewars Kata挑战](#第二部分)
#### 第一题：编码聚会1
```python
def count_developers(lst):
    # Your code here
    n=0
    for developer in lst:
        if developer['continent'] == 'Europe' and developer['language'] == 'JavaScript' :
            n+=1
    return n
```


#### 第二题： 使用函数进行计算
```python
def zero(func=None): 
    if func is None:
        return 0
    else:
        return func(0)
def one(func=None): 
    if func is None:
        return 1
    else:
        return func(1)
def two(func=None): 
    if func is None:
        return 2
    else:
        return func(2)
def three(func=None): 
    if func is None:
        return 3
    else:
        return func(3)
def four(func=None): 
    if func is None:
        return 4
    else:
        return func(4)
def five(func=None): 
    if func is None:
        return 5
    else:
        return func(5)
def six(func=None): 
    if func is None:
        return 6
    else:
        return func(6)
def seven(func=None):
    if func is None:
        return 7
    else:
        return func(7)
def eight(func=None):
    if func is None:
        return 8
    else:
        return func(8)
def nine(func=None): 
    if func is None:
        return 9
    else:
        return func(9)
def plus(x):
    return lambda y:y+x
def minus(x): 
    return lambda y:y-x
def times(x): 
    return lambda y:y*x

def divided_by(x): 
    return lambda y:y//x
```
#### 第三题： 缩短数值的过滤器(Number Shortening Filter)
```python
def shorten_number(base_values, base):
    def shortener(number):
        if isinstance(number, str) and number.isdigit():
            number = int(number)
            for i in range(len(base_values) - 1, -1, -1):
                divisor = base ** i
                if number >= divisor:
                    return f'{number // divisor}{base_values[i]}'
        return str(number)
    return shortener
```
#### 第四题： 编码聚会7
```python
def find_senior(lst): 
    # your code here
    result=[]
    result1=[]
    for developer in lst:
        result.append(developer['age'])
    ages=max(result)
    for developer in lst:
        if developer['age']==ages:
            result1.append(developer)
    return result1
```
#### 第五题： Currying versus partial application
```python
from inspect import signature
from functools import partial

def curry_partial(main_func, *args):
    
    if not(callable(main_func)):
        return main_func
    
    p = len(signature(main_func).parameters)
    func = partial(main_func)
    
    for a in args:
        if len(func.args) == p: break
        func = partial(func, a)
    
    if len(func.args) < p:
        return partial(curry_partial, main_func, *func.args)
    return func()
```
- [第三部分 使用Mermaid绘制程序流程图](#第三部分)
#### 第一题：编码聚会1
```mermaid
graph TD
    Start[Start] --> ForLoop[Enter Loop]
    ForLoop --> |For each developer| Condition[Check Condition]
    Condition --> |Condition Met| Increment[Increment Counter]
    Condition --> |Condition Not Met| Continue[Continue to Next Developer]
    Increment --> |Increment Counter| ForLoop
    Continue --> |Continue to Next Developer| ForLoop
    ForLoop --> |Loop Completed| End[End]
    End --> Output[Return Counter Value]

```
#### 第四题： 编码聚会7
```mermaid
graph TD
    Start[Start] --> InitializeResult[Initialize Result List]
    InitializeResult --> ForLoop1[Enter First Loop]
    ForLoop1 --> |For Each Developer| ExtractAge[Extract Age]
    ExtractAge --> |Extract Age| AppendAge[Append Age to Result List]
    AppendAge --> |Append Age| ForLoop1
    ForLoop1 --> |Complete First Loop| FindMaxAge[Find Max Age]
    FindMaxAge --> |Find Max Age| InitializeResult1[Initialize Result1 List]
    InitializeResult1 --> ForLoop2[Enter Second Loop]
    ForLoop2 --> |For Each Developer| CompareAge[Compare Age]
    CompareAge --> |Compare Age| AddToResult1[Add Matching Developers to Result1 List]
    AddToResult1 --> |Add to Result1| ForLoop2
    ForLoop2 --> |Complete Second Loop| End[End]
    End --> Output[Return Result1 List]
```
## 实验考查

请使用自己的语言并使用尽量简短代码示例回答下面的问题，这些问题将在实验检查时用于提问和答辩以及实际的操作。

1. 什么是函数式编程范式？
函数式编程范式（Functional Programming Paradigm）是一种编程方法论，它将计算看作是数学函数的组合。在函数式编程中，函数被视为一等公民，可以作为参数传递给其他函数，也可以从其他函数返回。它强调不可变性、无副作用和纯函数（相同输入始终产生相同输出），以及利用高阶函数来解决问题。函数式编程通常更加抽象和表达性，有助于编写清晰、简洁和可维护的代码。

2. 什么是lambda函数？请举例说明。
Lambda函数是匿名函数，也称为内联函数或函数字面量。它是一种在需要函数的地方定义短小的、临时的函数的方法，而不必使用传统的函数定义。Lambda函数通常用于函数式编程中，可以作为参数传递给其他函数。Lambda函数的一般形式是：`lambda arguments: expression`，其中 `arguments` 是函数的参数，`expression` 是函数的返回值。以下是一个Lambda函数的示例：
    ```python
        add = lambda x, y: x + y
        print(add(3, 5))  # 输出 8
        ```
3. 什么是高阶函数？常用的高阶函数有哪些？这些高阶函数如何工作？使用简单的代码示例说明。
高阶函数是可以接受一个或多个函数作为参数，并/或返回一个函数的函数。它们允许你在程序中操作函数，使代码更加灵活和抽象。常用的高阶函数包括：

   - `map(function, iterable)`: 将一个函数应用于可迭代对象的每个元素，并返回结果。例如：
     ```python
     numbers = [1, 2, 3, 4, 5]
     squared = list(map(lambda x: x ** 2, numbers))
     print(squared)  # 输出 [1, 4, 9, 16, 25]
     ```

   - `filter(function, iterable)`: 根据函数的条件过滤可迭代对象中的元素，并返回满足条件的元素。例如：
     ```python
     numbers = [1, 2, 3, 4, 5]
     even_numbers = list(filter(lambda x: x % 2 == 0, numbers))
     print(even_numbers)  # 输出 [2, 4]
     ```

   - `reduce(function, iterable)`: 递归地应用一个二元函数到可迭代对象中的元素，将它们合并为单个值。需要导入 `functools` 模块。例如：
     ```python
     from functools import reduce
     numbers = [1, 2, 3, 4, 5]
     product = reduce(lambda x, y: x * y, numbers)
     print(product)  # 输出 120 (1 * 2 * 3 * 4 * 5)
     ```
## 实验总结

总结一下这次实验你学习和使用到的知识，例如：编程工具的使用、数据结构、程序语言的语法、算法、编程技巧、编程思想。
在这次实验中，我学习和使用了以下知识和技能：
1. 我了解了Python中的数据结构，特别是列表（List）的用法，用于存储和操作多个元素的集合。
2. 程序语言的语法：我使用了Python语言的语法来编写函数和表达式，包括条件语句、循环、函数定义、Lambda函数等。
