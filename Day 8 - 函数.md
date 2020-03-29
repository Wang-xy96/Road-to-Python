
8.1 消息


```python
def display_message():
    print('You learn how to define a function in this chapter.')
display_message()
```

    You learn how to define a function in this chapter.
    

8.2 喜欢的图书


```python
def favorite_book(title):
    print('One of my favorite books ia ' + title.title())
favorite_book('Harry Potter')
```

    One of my favorite books ia Harry Potter
    

8.3 T恤


```python
def make_shirt(size,word):
    print("The size of this T-shirt is " + size)
    print('The words on T-shirt are '+ word)
make_shirt(size='S',word='I love China.')
```

    The size of this T-shirt is S
    The words on T-shirt are I love China.
    

8.4 大号T恤


```python
def make_shirt(size='Large',word='\'I love Python\''):
    print("The size of this T-shirt is " + size)
    print('The words on T-shirt are '+ word)
make_shirt()
```

    The size of this T-shirt is Large
    The words on T-shirt are 'I love Python'
    


```python
make_shirt(word='\'I love China\'')
```

    The size of this T-shirt is Large
    The words on T-shirt are 'I love China'
    

8.5 城市


```python
def describe_city(city,country='China'):
    print(city + ' is in ' + country)
describe_city('New York',country='US')
```

    New York is in US
    


```python
describe_city('Beijing')
describe_city('Shanghai')
```

    Beijing is in China
    Shanghai is in China
    

8.6 城市名


```python
def city_country(city,country):
    return city + ',' + country
print(city_country('Beijing','China'))
print(city_country('London','Britain'))
print(city_country('New York','U.S.A'))
```

    Beijing,China
    London,Britain
    New York,US
    

8.7 专辑


```python
def make_album(singer_name,album_name):
    album = {'name':singer_name,'album':album_name}
    return album
```


```python
a1 = make_album('Zhou Shen','Dalabengba')
print(a1)
a2 = make_album('Huahua','Qitian')
print(a2)
a3 = make_album('Hanhong','Tianlu')
print(a3)
```

    {'name': 'Zhou Shen', 'album': 'Dalabengba'}
    {'name': 'Huahua', 'album': 'Qitian'}
    {'name': 'Hanhong', 'album': 'Tianlu'}
    


```python
def make_album(singer_name,album_name,songs_num=""):
    album = {'name':singer_name,'album':album_name}
    if songs_num:
        album['songs'] = songs_num
    return album
```


```python
a1 = make_album('Zhou Shen','Dalabengba',5)
print(a1)
a2 = make_album('Huahua','Qitian',9)
print(a2)
a3 = make_album('Hanhong','Tianlu')
print(a3)
```

    {'name': 'Zhou Shen', 'album': 'Dalabengba', 'songs': 5}
    {'name': 'Huahua', 'album': 'Qitian', 'songs': 9}
    {'name': 'Hanhong', 'album': 'Tianlu'}
    

8.8 用户的专辑


```python
def make_album(singer_name,album_name):
    album = {'name':singer_name,'album':album_name}
    return album
while True:
    print("\nPlease tell me an album")
    print("(enter 'q' at any time to quit)") 
    s_name = input("Singer name: ")
    if s_name == 'q':
        break 
    a_name = input('Album name: ')
    if a_name == 'q':
        break
    album_li = make_album(s_name,a_name)
    print(album_li)
```


```python

```
