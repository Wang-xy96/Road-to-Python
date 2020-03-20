
3.1 姓名


```python
names = ['jane', 'rachael', 'chrystal','jennifer','jesicca']
print(names[0].title())
print(names[1].title())
print(names[2].title())
print(names[3].title())
print(names[4].title())
```

    Jane
    Rachael
    Chrystal
    Jennifer
    Jesicca
    

3.2 问候语


```python
message = 'have a good day!'
print(names[0].title()+ ','+ message)
print(names[1].title()+ ','+ message)
print(names[2].title()+ ','+ message)
print(names[3].title()+ ','+ message)
print(names[4].title()+ ','+ message)
```

    Jane,have a good day!
    Rachael,have a good day!
    Chrystal,have a good day!
    Jennifer,have a good day!
    Jesicca,have a good day!
    

3.3 访问自己的列表


```python
names.append('ben') #使用append()在列表末尾添加元素
names
```




    ['jane', 'rachael', 'chrystal', 'jennifer', 'jesicca', 'ben']




```python
names.insert(0,'tony') #insert()可以在列表的任何位置添加新元素
names
```




    ['tony', 'jane', 'rachael', 'chrystal', 'jennifer', 'jesicca', 'ben']



删除：
1. 使用del可删除列表任何位置处的元素
2. 使用方法pop()可以删除列表末尾的元素，也可以删除指定位置的元素
3. 如果你不知道元素的位置的话，使用remove()可以直接删除列表中的值
如何区别del和pop()：如果你要从列表中删除一个元素，且不再以任何方式使用它，就使用del语句；如果你要删除元素后还要继续使用它，就使用方法pop()


```python
del names[0]
print(names)
```

    ['jane', 'rachael', 'chrystal', 'jennifer', 'jesicca', 'ben']
    


```python
best_friend = names.pop(0)
best_friend
```




    'jane'




```python
friend = 'rachael'
names.remove(friend)
print(names)
```

    ['chrystal', 'jennifer', 'jesicca', 'ben']
    

3.4 嘉宾名单


```python
name_1 = ['father','mother','brother','jane','rachael','jennifer']
print('I would like to invite' + name_1[3].title() + ',' + name_1[4].title() + ',and ' + name_1[5].title() + ' to have dinner with me')
```

    I would like to inviteJane,Rachael,and Jennifer to have dinner with me
    

3.5 修改嘉宾名单


```python
print(name_1[5].title() + ' is unable to come.')
name_1.remove('jennifer')
name_1.append('ben')
name_1
print('I would like to invite' + name_1[3] + ' to have dinner with me.') 
```

    Jennifer is unable to come.
    I would like to invitejane to have dinner with me.
    

3.6 添加嘉宾


```python
#I find a bigger table so that I can invite more to have dinner with me
name_1.insert(0,'tony')
name_1.insert(4,'ranger')
name_1.append('nina')
name_1
```




    ['tony',
     'father',
     'mother',
     'brother',
     'ranger',
     'jane',
     'rachael',
     'ben',
     'nina']




```python
print('Due to the delayed delivery of new table, I could only invite two people to have dinner with me.') 
p1 = name_1.pop()
print(p1 + ", I am so sorry that I can't invite you to dinner.")
p2 = name_1.pop()
print(p2 + ", I am so sorry that I can't invite you to dinner.")
p3 = name_1.pop()
print(p3 + ", I am so sorry that I can't invite you to dinner.")
p4 = name_1.pop()
print(p4 + ", I am so sorry that I can't invite you to dinner.")
p5 = name_1.pop()
print(p5 + ", I am so sorry that I can't invite you to dinner.")
p6 = name_1.pop()
print(p6 + ", I am so sorry that I can't invite you to dinner.")
p7 = name_1.pop()
print(p7 + ", I am so sorry that I can't invite you to dinner.")
del name_1[0]
del name_1[0]
print(name_1)
```

    Due to the delayed delivery of new table, I could only invite two people to have dinner with me.
    nina, I am so sorry that I can't invite you to dinner.
    ben, I am so sorry that I can't invite you to dinner.
    rachael, I am so sorry that I can't invite you to dinner.
    jane, I am so sorry that I can't invite you to dinner.
    ranger, I am so sorry that I can't invite you to dinner.
    brother, I am so sorry that I can't invite you to dinner.
    mother, I am so sorry that I can't invite you to dinner.
    []
    

3.8 放眼世界


```python
places = ['Singapore','Russia','Italy','Fance','Germany']
print(places)
```

    ['Singapore', 'Russia', 'Italy', 'Fance', 'Germany']
    


```python
print(sorted(places))
```

    ['Fance', 'Germany', 'Italy', 'Russia', 'Singapore']
    


```python
print(places)
```

    ['Singapore', 'Russia', 'Italy', 'Fance', 'Germany']
    


```python
print(sorted(places,reverse = True))
```

    ['Singapore', 'Russia', 'Italy', 'Germany', 'Fance']
    


```python
print(places)
```

    ['Singapore', 'Russia', 'Italy', 'Fance', 'Germany']
    


```python
places.reverse()
print(places)
```

    ['Germany', 'Fance', 'Italy', 'Russia', 'Singapore']
    


```python
places.reverse()
print(places)
```

    ['Singapore', 'Russia', 'Italy', 'Fance', 'Germany']
    


```python
places.sort()
print(places)
```

    ['Fance', 'Germany', 'Italy', 'Russia', 'Singapore']
    


```python
places.sort(reverse=True)
print(places)
```

    ['Singapore', 'Russia', 'Italy', 'Germany', 'Fance']
    

3.9 晚餐嘉宾


```python
len(name_1)
```




    6



3.10 尝试使用各个函数


```python
city = ['Beijing','Shanghai','Guilin','Nanjing','Shenzhen']
```


```python
city[2]
print('My hometown is the city of ' + city[2] + '.')
```

    My hometown is the city of Guilin.
    


```python
city[4] = 'Hongkong'
city
```




    ['Beijing', 'Shanghai', 'Guilin', 'Nanjing', 'Hongkong']




```python
city.append('Tianjing')
city
```




    ['Beijing', 'Shanghai', 'Guilin', 'Nanjing', 'Hongkong', 'Tianjing']




```python
city.insert(2,'Xian')
city
```




    ['Beijing', 'Shanghai', 'Xian', 'Guilin', 'Nanjing', 'Hongkong', 'Tianjing']




```python
del city[3]
city
```




    ['Beijing', 'Shanghai', 'Xian', 'Nanjing', 'Hongkong', 'Tianjing']




```python
capital = city.pop(0)
print('The Capital city of China is ' + capital + '.')
```

    The Capital city of China is Beijing.
    


```python
city.remove('Nanjing')
city
```




    ['Shanghai', 'Xian', 'Hongkong', 'Tianjing']




```python
city.sort()
print(city)
```

    ['Hongkong', 'Shanghai', 'Tianjing', 'Xian']
    


```python
city.sort(reverse=True)
print(city)
```

    ['Xian', 'Tianjing', 'Shanghai', 'Hongkong']
    


```python
sorted(city,reverse=True)
```




    ['Xian', 'Tianjing', 'Shanghai', 'Hongkong']




```python
sorted(city)
```




    ['Hongkong', 'Shanghai', 'Tianjing', 'Xian']




```python
print(city)
```

    ['Xian', 'Tianjing', 'Shanghai', 'Hongkong']
    


```python
len(city)
```




    4




```python

```
