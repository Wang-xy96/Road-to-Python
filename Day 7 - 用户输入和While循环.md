
7.1 汽车租赁


```python
message = input('What band of car do you want to rent? ')
print('Let me see if I can find you a ' + message)
```

    What band of car do you want to rent? Subaru
    Let me see if I can find you a Subaru
    

7.2 餐馆订位


```python
num = input("How many people will dine in? ")
if int(num) < 8:
    print('There are tables available.')
else:
    print('There are no table available.')
```

    How many people will dine in? 8
    There are no table available.
    

7.3 10的整数倍


```python
number = input('Please enter a number: ')
if int(number) % 10 == 0:
    print('This number is a integral multiple of 10.')
else:
    print('This number is not a integral multiple of 10.')
```

    Please enter a number: 10
    This number is a integral multiple of 10.
    

7.4 比萨配料


```python
pizza_toppings = "\nPlease choose pizza toppings: "
message = ""
while message != "quit":
    message = input(pizza_toppings)
    
    if message != 'quit':
        print(message + 'will be added to your pizza.')
```

    
    Please choose pizza toppings: pepperoni
    pepperoniwill be added to your pizza.
    
    Please choose pizza toppings: quit
    

7.5 电影票


```python
while True:
    age = int(input('What is your age?'))
    if age < 3:
        print('For free')
    elif 3 <= age <= 12:
        print('The ticket costs 10 dollars.')
    elif age > 12:
        print('The ticket costs 15 dollars.')
    else:
        print('Wrong message!')
        break
```

    What is your age?7
    The ticket costs 10 dollars.
    What is your age?14
    The ticket costs 15 dollars.
    What is your age?2
    For free
    What is your age?e
    


    ---------------------------------------------------------------------------

    ValueError                                Traceback (most recent call last)

    <ipython-input-2-e857c8929aa7> in <module>
          1 while True:
    ----> 2     age = int(input('What is your age?'))
          3     if age < 3:
          4         print('For free')
          5     elif 3 <= age <= 12:
    

    ValueError: invalid literal for int() with base 10: 'e'


7.8 熟食店


```python
sandwich_orders = ['tuna sandwich','chicken sandwich','beef sandwich','super sandwich']
finished_sandwiches = []
while sandwich_orders:
    sandwich_made = sandwich_orders.pop()
    print('I made you ' + sandwich_made)
    finished_sandwiches.append(sandwich_made)
    
print("\nAll sandwiches have been made.")
for finished_sandwich in finished_sandwiches:
    print(finished_sandwich)
```

    I made you super sandwich
    I made you beef sandwich
    I made you chicken sandwich
    I made you tuna sandwich
    
    All sandwiches have been made.
    super sandwich
    beef sandwich
    chicken sandwich
    tuna sandwich
    

7.9 五香烟熏牛肉（pastrami)卖完了


```python
sandwich_orders = ['tuna sandwich','pastrami','chicken sandwich','pastrami','beef sandwich','super sandwich','pastrami']
print("\nAll pastrami has been sold out.")
while 'pastrami' in sandwich_orders:
    sandwich_orders.remove('pastrami')
print(sandwich_orders)
```

    
    All pastrami has been sold out.
    ['tuna sandwich', 'chicken sandwich', 'beef sandwich', 'super sandwich']
    

7.10 梦想的度假胜地


```python
responses = {}
polling_active = True
while polling_active:
    name = input("\nWhat is your name? ")
    response = input("\nIf you could visit one place in the world, where would you go? ")
    responses[name] = response
```
