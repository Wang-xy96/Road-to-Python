
9.1 餐馆


```python
class Restaurant():
    def __init__(self,restaurant_name,cuisine_type):
        self.name = restaurant_name
        self.type = cuisine_type     
    def describe_restaurant(self):
        print("The name of the restaurant is " + self.name.title())
        print("The cuisine type is " + self.type.title())     
    def open_restaurant(self):
        print(self.name.title() + " is now open!")   
        
my_restaurant = Restaurant('肯德基','快餐')
my_restaurant.describe_restaurant()
my_restaurant.open_restaurant()
```

    The name of the restaurant is 肯德基
    The cuisine type is 快餐
    肯德基 is now open!
    

9.2 三家餐馆


```python
class Restaurant():
    restaurant_1 = Restaurant('小龙坎','火锅')
    restaurant_1.describe_restaurant()
    restaurant_2 = Restaurant('海底捞','火锅')
    restaurant_2.describe_restaurant()
    restaurant_3 = Restaurant('狗不理包子','包子铺')
    restaurant_3.describe_restaurant()
```

    The name of the restaurant is 小龙坎
    The cuisine type is 火锅
    The name of the restaurant is 海底捞
    The cuisine type is 火锅
    The name of the restaurant is 狗不理包子
    The cuisine type is 包子铺
    

9.3 用户


```python
class User():
    def __init__(self,first_name,last_name,age,gender):
        self.name = first_name + last_name
        self.age = age
        self.gender = gender
        
    def describe_user(self):
        print('Name is ' + self.name.title())
        print('Age is ' + self.age.title())
        print('Gender is ' + self.gender.title())
    
    def greet_user(self):
        print("Hello " + self.name.title() + " !")
        
user_1 = User('Anita','Wang','23','Female')
user_1.describe_user()
user_1.greet_user()
```

    Name is Anitawang
    Age is 23
    Gender is Female
    Hello Anitawang !
    

9.4 就餐人数


```python
class Restaurant():
    def __init__(self,restaurant_name,cuisine_type):
        self.name = restaurant_name
        self.type = cuisine_type
        self.number_served = 2
    def describe_restaurant(self):
        print("The name of the restaurant is " + self.name.title())
        print("The cuisine type is " + self.type.title())     
    def open_restaurant(self):
        print(self.name.title() + " is now open!")   
    def read_number_served(self):
        
        
my_restaurant = Restaurant('肯德基','快餐')
my_restaurant.read_number_served()
```

    This restaurant has 2 customers.
    


```python
class Restaurant():
    def __init__(self,restaurant_name,cuisine_type):
        self.name = restaurant_name
        self.type = cuisine_type
        self.number_served = 2
    def describe_restaurant(self):
        print("The name of the restaurant is " + self.name.title())
        print("The cuisine type is " + self.type.title())     
    def open_restaurant(self):
        print(self.name.title() + " is now open!")
    def set_number_served(self,number):
        self.number_served = number
    def read_number_served(self):
        print('This restaurant has '+ str(self.number_served) + ' customers.')
    
my_restaurant = Restaurant('肯德基','快餐')
my_restaurant.set_number_served(8)
my_restaurant.read_number_served()
```

    This restaurant has 8 customers.
    


```python
class Restaurant():
    def __init__(self,restaurant_name,cuisine_type):
        self.name = restaurant_name
        self.type = cuisine_type
        self.number_served = 2
    def describe_restaurant(self):
        print("The name of the restaurant is " + self.name.title())
        print("The cuisine type is " + self.type.title())     
    def open_restaurant(self):
        print(self.name.title() + " is now open!")
    def set_number_served(self,number):
        self.number_served = number
    def increment_number_served(self,increment_number):
        self.number_served += increment_number
    def read_number_served(self):
        print('This restaurant has '+ str(self.number_served) + ' customers.')
my_restaurant = Restaurant('肯德基','快餐')
my_restaurant.set_number_served(9)
my_restaurant.increment_number_served(8)
my_restaurant.read_number_served()
```

    This restaurant has 17 customers.
    

9.5 尝试登陆次数


```python
class User():
    def __init__(self,first_name,last_name,age,gender):
        self.name = first_name + last_name
        self.age = age
        self.gender = gender
        self.login_attempts = 0
        
    def describe_user(self):
        print('Name is ' + self.name.title())
        print('Age is ' + self.age.title())
        print('Gender is ' + self.gender.title())
    
    def greet_user(self):
        print("Hello " + self.name.title() + " !")
        
    def increment_login_attempts(self):
        self.login_attempts += 1
    
    def reset_login_attempts(self):
        self.login_attempts= 0
        
user_1 = User('Anita','Wang','23','Female')
user_1.increment_login_attempts()
print(user_1.login_attempts)
user_1.increment_login_attempts()
user_1.increment_login_attempts()
print(user_1.login_attempts)
user_1.reset_login_attempts()
print(user_1.login_attempts)
```

    1
    3
    0
    
