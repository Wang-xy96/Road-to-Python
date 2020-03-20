

```python
message = "Hello Python World!"
print(message)

message = "Hello Python Crash Course World!"
print(message)
```

    Hello Python World!
    Hello Python Crash Course World!
    


```python
name = 'ada lovelace'
print(name.title())
```

    Ada Lovelace
    


```python
name = 'Ada Lovelace'
print(name.upper())
print(name.lower())
```

    ADA LOVELACE
    ada lovelace
    

拼接


```python
first_name = "ada"
last_name = 'lovelace'
full_name = first_name + ' ' + last_name
print(full_name)
```

    ada lovelace
    


```python
print('Hello, '+ full_name.title()+ "!")
```

    Hello, Ada Lovelace!
    


```python
print('Languages:\n\tPython\n\tC\n\tJacaScript')#\t是制表符，\n是换行符
```

    Languages:
    	Python
    	C
    	JacaScript
    


```python
favorite_language = 'Python ' #rstrip()删除末尾的空白
favorite_language = favorite_language.rstrip()
favorite_language
```




    'Python'




```python
favorite_language = ' Python' #lstrip()删除开头的空白
favorite_language = favorite_language.lstrip()
favorite_language
```




    'Python'




```python
favorite_language = ' Python ' #strip()删除字符串两端的空白
favorite_language = favorite_language.strip()
favorite_language
```




    'Python'



练习：个性化消息


```python
name = 'Eric'
print('Hello '+ name + ', would you like to learn some Python today?')
```

    Hello Eric, would you like to learn some Python today?
    

练习：调整名字的大小写


```python
name2 = 'anita wang'
print(name2.title())
print(name2.upper())
print(name2.lower())
```

    Anita Wang
    ANITA WANG
    anita wang
    

练习：名言


```python
print('Albert Einstein once said, "A person who never made a mistake never trieed anything new."')
```

    Albert Einstein once said, "A person who never made a mistake never trieed anything new."
    

练习：名言2


```python
famous_person = 'Albert Einstein'
message = '"A person who never made a mistake never tried anything new."' 
print(famous_person + " once said," + message)
```

    Albert Einstein once said,"A person who never made a mistake never tried anything new."
    

剔除人名中的空白


```python
name3 = " Rita\n\tWang "
print(name3)
```

     Rita
    	Wang 
    


```python
print(name3.lstrip())
print(name3.rstrip())
print(name3.strip())
```

    Rita
    	Wang 
     Rita
    	Wang
    Rita
    	Wang
    

两个乘号表示乘方运算


```python
3**2
```




    9




```python
3**3
```




    27




```python
3**6
```




    729



数字8


```python
print(5+3)
print(10-2)
print(2*4)
print(int(16/2))
```

    8
    8
    8
    8
    

最喜欢的数字


```python
favorite_number = 6
message = 'My favorite number is '
print(message + str(favorite_number))
```

    My favorite number is 6
    


```python
import this
```

    The Zen of Python, by Tim Peters
    
    Beautiful is better than ugly.
    Explicit is better than implicit.
    Simple is better than complex.
    Complex is better than complicated.
    Flat is better than nested.
    Sparse is better than dense.
    Readability counts.
    Special cases aren't special enough to break the rules.
    Although practicality beats purity.
    Errors should never pass silently.
    Unless explicitly silenced.
    In the face of ambiguity, refuse the temptation to guess.
    There should be one-- and preferably only one --obvious way to do it.
    Although that way may not be obvious at first unless you're Dutch.
    Now is better than never.
    Although never is often better than *right* now.
    If the implementation is hard to explain, it's a bad idea.
    If the implementation is easy to explain, it may be a good idea.
    Namespaces are one honking great idea -- let's do more of those!
    


```python

```
