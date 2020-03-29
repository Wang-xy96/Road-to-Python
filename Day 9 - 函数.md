
8.9 魔术师


```python
def show_magicians(magicians_names):
    for name in magicians_names:
        print(name)
names = ['Anita','Nina','Jane']
show_magicians(names)
```

    Anita
    Nina
    Jane
    

8.10 了不起的魔术师


```python
magicians = ['Anita','Nina','Jane']
great_magicians = []
def make_great(magicians,great_magicians):
    while magicians:
        magician = magicians.pop()
        great_magician = 'the Great ' + magician
        great_magicians.append(great_magician)
        
def show_magicians(great_magicians):
    for name in great_magicians:
        print(name)
        
make_great(magicians,great_magicians)
show_magicians(great_magicians)
```

    the Great Jane
    the Great Nina
    the Great Anita
    

8.11 不变的魔术师


```python
magicians = ['Anita','Nina','Jane']
great_magicians = []
def make_great(magicians,great_magicians):
    while magicians:
        magician = magicians.pop()
        great_magician = 'the Great ' + magician
        great_magicians.append(great_magician)
        
def show_magicians(great_magicians):
    for name in great_magicians:
        print(name)
        
make_great(magicians[:],great_magicians)
show_magicians(great_magicians)
show_magicians(magicians)
```

    the Great Jane
    the Great Nina
    the Great Anita
    Anita
    Nina
    Jane
    

8.12 三明治


```python
def make_sandwich(*toppings):
    print("\nThe customer has ordered: ")
    for topping in toppings:
        print('- ' + topping)
make_sandwich('tuna','avocado','mango')
```

    
    The customer has ordered: 
    - tuna
    - avocado
    - mango
    

8.13 用户简介


```python
def build_profile(first, last, **user_info):
    profile = {}
    profile['first_name'] = first
    profile['last_name'] = last
    for key,value in user_info.items():
        profile[key] = value
    return profile
user_profile = build_profile('Anita','Wang',location='China',gender='Female',age='23')
print(user_profile)
```

    {'first_name': 'Anita', 'last_name': 'Wang', 'location': 'China', 'gender': 'Female', 'age': '23'}
    

8.14 汽车


```python
def make_car(maker,model,**car_info):
    profile = {}
    profile['Maker'] = maker
    profile['Model'] = model
    for key,value in car_info.items():
        profile[key] = value
    return profile
car = make_car('subaru','outback',color = 'blue',tow_package=True)
print(car)
```

    {'Maker': 'subaru', 'Model': 'outback', 'color': 'blue', 'tow_package': True}
    
