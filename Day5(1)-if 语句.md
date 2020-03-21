
5.8 以特殊的方式跟管理员打招呼


```python
user_name = ['Michael','Stella','Nina','Ben','Admin']
for name in user_name:
    if name == 'Admin':
        print('Hello ' + name + ', whould you like to see a statur report?')
    else:
        print('Hello ' + name + ', thank you for logging in again.')
```

    Hello Michael, thank you for logging in again.
    Hello Stella, thank you for logging in again.
    Hello Nina, thank you for logging in again.
    Hello Ben, thank you for logging in again.
    Hello Admin, whould you like to see a statur report?
    

5.9 处理没有用户的情形


```python
user_name = []
if user_name:
    for name in user_name:
        print('Hello ' + name + ', whould you like to see a statur report?')
else:
     print('We need to find some users!')   
```

    We need to find some users!
    

**5-10 检车用户名，确保比较时不区分大小写，先把所有的元素变成小写储存在新的列表中，然后再比较


```python
current_users = ['Anita','Jane','Rachael','Ben','Tony']
new_users = ['Stella','Nina','Ben','TONY','Jay']
current_users_lower = [current_user.lower() for current_user in current_users]
new_users_lower = [new_user.lower() for new_user in new_users]
print(current_users_lower)
print(new_users_lower)
```

    ['anita', 'jane', 'rachael', 'ben', 'tony']
    ['stella', 'nina', 'ben', 'tony', 'jay']
    


```python
for new_user in new_users_lower:
    if new_user in current_users_lower:
        print('This name has been occupied, please enter a new one.')
    else:
        print('This name has not been used.')
```

    This name has not been used.
    This name has not been used.
    This name has been occupied, please enter a new one.
    This name has been occupied, please enter a new one.
    This name has not been used.
    

5.11 序列


```python
numbers = [1,2,3,4,5,6,7,8,9]
for number in numbers:
    if number >= 4:
        print(str(number) + 'th')
    elif number == 3:
        print(str(number) + 'rd')
    elif number == 2:
        print(str(number) + 'nd')
    else:
        print(str(number) + 'st')
```

    1st
    2nd
    3rd
    4th
    5th
    6th
    7th
    8th
    9th
    


```python

```
