
5.1 条件测试


```python
car = 'subaru'
print("Is car == 'subaru'? I predict True.")
print(car == 'subaru')

print("\nIs car == 'audi'? I predict False.")
print(car == 'audi')
```

    Is car == 'subaru'? I predict True.
    True
    
    Is car == 'audi'? I predict False.
    False
    


```python
food = 'rice'
print("Is food == 'rice'? I predict True.")
print(food == 'rice')

print("\nIs food == 'noodle'? I predict False.")
print(car == 'noodle')
```

    Is food == 'rice'? I predict True.
    True
    
    Is food == 'noodle'? I predict False.
    False
    

5.2 更多的测试


```python
p1 = 'car'
p2 = 'food'
print(p1 == p2)
p1 == p2
```

    False
    




    False




```python
name = 'Karl'
name1 = 'KarL'
print(name.lower() == name1.lower())
```

    True
    


```python
3 == 5
```




    False




```python
3 != 5
```




    True




```python
3 > 5
```




    False




```python
3 < 5
```




    True




```python
3 <= 5
```




    True




```python
3 >= 5
```




    False




```python
age_0 = 18
age_1 = 23
age_0 > 18 and age_1 < 25
```




    False




```python
age_0 = 18
age_1 = 23
age_0 > 18 or age_1 < 25
```




    True




```python
food = ['noodle','rice','beef','pork']
print('noodle' in food)
print('milk' in food)
```

    True
    False
    


```python
food = ['noodle','rice','cake','pork']
print('beef' not in food)
```

    True
    


```python

```
