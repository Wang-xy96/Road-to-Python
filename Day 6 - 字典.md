
6.1 人


```python
information = {'first_name': 'San', 'last_name': 'Zhang','age': 24,'city': 'Shanghai'}
print(information['first_name'])
print(information['last_name'])
print(information['age'])
print(information['city'])
```

    San
    Zhang
    24
    Shanghai
    

6.2 喜欢的数字


```python
favorite_number = {
    'Zhang San': 6,
    'Li Si': 9,
    'Wang Wu': 7,
    'Xie Guangkun': 3,
    'Xie Dajiao': 2
    }
print("Zhang San's favorite number is " + str(favorite_number['Zhang San']))
print("Li Si's favorite number is " + str(favorite_number['Li Si']))
print("Wang Wu's favorite number is " + str(favorite_number['Wang Wu']))
print("Xie Guangkun's favorite number is " + str(favorite_number['Xie Guangkun']))
print("Xie Dajiao's favorite number is " + str(favorite_number['Xie Dajiao']))
```

    Zhang San's favorite number is 6
    Li Si's favorite number is 9
    Wang Wu's favorite number is 7
    Xie Guangkun's favorite number is 3
    Xie Dajiao's favorite number is 2
    

6.3 词汇表


```python
vocabulary = {
    'lower()':'将字符全部变成小写',
    'upper()':'将字符串全部变成大写',
    'title()':'将每个单词的首字母变成大写',
    'len()':'字符串的长度',
    'str()':'将其他的类型变成字符串'
    }
```


```python
print('lower():\n' +  
      vocabulary['lower()'])
print('upper():\n'+
    vocabulary['upper()'])
print('title():\n'+
    vocabulary['title()'])
print('len():\n'+
    vocabulary['len()'])
print('str():\n'+
    vocabulary['str()'])
```

    lower():
    将字符全部变成小写
    upper():
    将字符串全部变成大写
    title():
    将每个单词的首字母变成大写
    len():
    字符串的长度
    str():
    将其他的类型变成字符串
    

6.4 词汇表2


```python
for key,value in vocabulary.items():
    print(key + ':' + value)
```

    lower():将字符全部变成小写
    upper():将字符串全部变成大写
    title():将每个单词的首字母变成大写
    len():字符串的长度
    str():将其他的类型变成字符串
    

6.5 河流


```python
rivers = {'nile':'egypt','Yangtze':'China','Mississipi':'America'}
for key,value in rivers.items():
    print('The ' + key + ' runs through ' + value)
```

    The nile runs through egypt
    The Yangtze runs through China
    The Mississipi runs through America
    


```python
rivers = {'nile':'egypt','Yangtze':'China','Mississipi':'America'}
for key in rivers.keys():
    print(key.title())
```

    Nile
    Yangtze
    Mississipi
    


```python
for value in rivers.values():
    print(value.title())
```

    Egypt
    China
    America
    

6.6 调查


```python
favorite_languages = {
    'jen':'python',
    'sarah':'c',
    'edward':'ruby',
    'phil':'python'
}
name_li = ['jen','edward','anita','jane']
for name in name_li:
    print(name.title())
    if name in favorite_languages.keys():
        print('Thank you!')
    if name not in favorite_languages.keys():
        print('Invite you to enroll in investigation.')
```

    Jen
    Thank you!
    Edward
    Thank you!
    Anita
    Invite you to enroll in investigation.
    Jane
    Invite you to enroll in investigation.
    

6.7 人


```python
people ={
    'Zsan':{
    'first': 'San', 
    'last': 'Zhang',
    'age': 24,
    'city': 'Shanghai'    
    },
    'Wwu':{
    'first':'Wu',
    'last':'Wang',
    'age':22,
    'city':'Guangzhou'
    },
    'Lsi':{
    'first':'Si',
    'last':'Li',
    'age':19,
    'city':'Chengdu'
    }
}
```


```python
for name,name_info in people.items():
    print("\nusername: " + name)
    full_name = name_info['first'] + "" + name_info['last']
    city = name_info['city']
    age = name_info['age']
    print("\tFull name: " + full_name.title())
    print("\tAge: " + str(name_info['age']))
    print("\tCity: " + city)
```

    
    username: Zsan
    	Full name: Sanzhang
    	Age: 24
    	City: Shanghai
    
    username: Wwu
    	Full name: Wuwang
    	Age: 22
    	City: Guangzhou
    
    username: Lsi
    	Full name: Sili
    	Age: 19
    	City: Chengdu
    

6.8 宠物


```python
mimi = {'type':'cat','owner':'Anita'}
jojo = {'type':'dog','owner':'Lily'}
momoko = {'type':'cat','owner':'Sue'}
pets = [mimi,jojo,momoko]
for pet in pets:
    print(pet)
```

    {'type': 'cat', 'owner': 'Anita'}
    {'type': 'dog', 'owner': 'Lily'}
    {'type': 'cat', 'owner': 'Sue'}
    

6.9 喜欢的地方


```python
favorite_places = {
    'Jane':['Egypt','Norway','Beijing'],
    'Anita':['Guilin','Iceland','Shanghai'],
    'Rachael':['Singapore','Beijing','France']
}
for name,places in favorite_places.items():
    print("\n" + name.title() + "'s favorite places are:")
    for place in places:
        print("\t" + place.title())
```

    
    Jane's favorite places are:
    	Egypt
    	Norway
    	Beijing
    
    Anita's favorite places are:
    	Guilin
    	Iceland
    	Shanghai
    
    Rachael's favorite places are:
    	Singapore
    	Beijing
    	France
    

6.10 喜欢的数字


```python
favorite_number = {
    'Zhang San': [6,8,10,26],
    'Li Si':[9,33,99,88,66],
    'Wang Wu': [7,100,55],
    'Xie Guangkun': [3,286],
    'Xie Dajiao': [2,999,2020]
    }
for name,numbers in favorite_number.items():
    print("\n" + name + "'s favorite numbers are:")
    for number in numbers:
        print("\t" + str(number))
```

    
    Zhang San's favorite numbers are:
    	6
    	8
    	10
    	26
    
    Li Si's favorite numbers are:
    	9
    	33
    	99
    	88
    	66
    
    Wang Wu's favorite numbers are:
    	7
    	100
    	55
    
    Xie Guangkun's favorite numbers are:
    	3
    	286
    
    Xie Dajiao's favorite numbers are:
    	2
    	999
    	2020
    

6.11 城市


```python
cities = {
    'Guilin':{
    'country':'China',
    'population':'250万',
    'fact':"世界闻名的旅游城市"
    },
    'Denver':{
    'country':'USA',
    'population':'unkown',
    'fact':"The capital city of Colorado"
    },
    'London':{
    'country':'Britain',
    'population':'2000000',
    'fact':"The place where stands the london eye."
    },
}
for city,info in cities.items():
    print("\nCity: "+ city)
    Country = info['country']
    Population = info['population']
    Fact = info['fact']
    print("\tCountry: "+ Country)
    print("\tPopulation: " + Population)
    print("\tFact: " + Fact)
```

    
    City: Guilin
    	Country: China
    	Population: 250万
    	Fact: 世界闻名的旅游城市
    
    City: Denver
    	Country: USA
    	Population: unkown
    	Fact: The capital city of Colorado
    
    City: London
    	Country: Britain
    	Population: 2000000
    	Fact: The place where stands the london eye.
    
