# **Python for Beginners**

---

## **1. Variables & Data Types**

### **Variables & Naming Rules**

```python
company_name = "TechCorp"    # lowercase with underscores
employeeCount = 120          # camelCase (less common in Python)
FOUNDED_YEAR = 2010          # constants are usually UPPERCASE
```

### **Primitive Types**

```python
product_name = "Laptop"      # str
price = 45000                # int
rating = 4.7                 # float
is_available = True          # bool
discount = None              # None
z = 3 + 5j                   # complex number
```

### **Reference Types**

```python
categories = ["Electronics", "Clothing"]      # list
features = ("Lightweight", "Portable")        # tuple
product = {"name": "Mouse", "price": 499}     # dict
tags = {"sale", "new", "popular"}             # set

def calculate_gst(amount): return amount * 0.18  # function

class Item: pass                                 # object
```

---

## **2. Operators**

### **Arithmetic**

```python
revenue = 10000
expenses = 4000
profit = revenue - expenses   # 6000
```

### **Assignment**

```python
profit += 500   # Adds bonus → 6500
```

### **Comparison**

```python
print(profit > 5000)   # True
```

### **Logical**

```python
has_stock = True
is_online = False
print(has_stock and is_online)  # False
```

### **Membership**

```python
print("Laptop" in ["Laptop", "Phone"])   # True
```

### **Identity**

```python
x = [1, 2, 3]
y = x
print(x is y)      # True
print(x is not y)  # False
```

### **Ternary**

```python
status = "High Profit" if profit > 5000 else "Low Profit"
print(status)   # High Profit
```

---

## **3. Control Structures**

### **Conditional**

```python
rating = 4.5
if rating >= 4.5:
    print("Excellent product")
elif rating >= 3.5:
    print("Good product")
else:
    print("Average product")
```

### **Pattern Matching (Python 3.10+)**

```python
payment_method = "UPI"

match payment_method:
    case "Credit Card":
        print("Processing via Credit Card")
    case "UPI":
        print("Processing via UPI")
    case _:
        print("Payment method not supported")
```

### **Loops**

```python
products = ["Laptop", "Phone", "Tablet"]

# for loop
for p in products:
    print(p)

# while loop
i = 0
while i < 2:
    print("Offer available")
    i += 1
```

### **Loop Controls**

```python
for p in products:
    if p == "Phone": continue   # skip
    if p == "Tablet": break     # stop
    print(p)
```

### **Helpers**

```python
for i in range(3): print(i)                   # 0,1,2
for i, item in enumerate(products): print(i, item)
for a, b in zip([1,2,3], ["a","b","c"]): print(a, b)
```

---

## **4. Functions**

### **Definition**

```python
def greet_customer(name):
    return f"Hello {name}, welcome to TechStore!"
```

### **Default Parameters**

```python
def shipping_charge(location="India"):
    return 50 if location == "India" else 200
```

### **\*args & \*\*kwargs**

```python
def order_summary(*items, **details):
    return f"Items: {items}, Details: {details}"

print(order_summary("Laptop", "Mouse", customer="Alice"))
```

### **Lambda**

```python
discount = lambda price: price * 0.9
print(discount(1000))
```

### **Higher-Order Functions**

```python
from functools import reduce
prices = [100, 200, 300]

print(list(map(lambda p: p*2, prices)))
print(list(filter(lambda p: p>150, prices)))
print(reduce(lambda a,b: a+b, prices))
```

### **Scope**

```python
x = 10

def outer():
    global x
    x = 20
    def inner():
        nonlocal y
        y = 30
    y = 25
    inner()
    print("y inside:", y)

outer()
print("x outside:", x)
```

### **Recursion**

```python
def factorial(n):
    return 1 if n==0 else n * factorial(n-1)

print(factorial(5))   # 120
```

---

## **5. Strings**

```python
customer = "   Alice Johnson   "

# Properties
print(len(customer))
print(customer[2])
print(customer[0:5])

# Searching
print(customer.find("John"))
print(customer.count("o"))

# Modification
print(customer.upper())
print(customer.strip())
print(customer.replace("Alice", "Bob"))

# Checking
print(customer.startswith("Alice"))
print("123".isdigit())
print("abc".isalpha())

# Formatting
order_id = 101
print(f"Order ID: {order_id} for {customer.strip()}")
print("Order ID: {} for {}".format(order_id, customer.strip()))
print("Order ID: %d for %s" % (order_id, customer.strip()))

# Split & Join
skills = "Python,Java,SQL".split(",")
print(" | ".join(skills))

# Immutability
text = "Hello"
# text[0] = "h"   ❌ (not allowed)
```

---

## **6. Lists**

```python
cart = ["Laptop", "Phone"]

# Add/Remove
cart.append("Mouse")
cart.insert(1, "Tablet")
cart.pop()
cart.remove("Phone")

# Search
print("Laptop" in cart)
print(cart.index("Laptop"))

# Transform
numbers = [3,1,2]
numbers.sort()
numbers.reverse()
print([n*2 for n in numbers])

# Nested
matrix = [[1,2], [3,4]]

# Copy vs Reference
a = [1,2,3]
b = a
c = a.copy()
a.append(4)
print(b)  # [1,2,3,4]
print(c)  # [1,2,3]

# Combine
list1 = [1,2]
list2 = [3,4]
print(list1 + list2)
```

---

## **7. Tuples**

```python
coords = (10, 20)
print(coords[0])

# Unpacking
x, y = coords
print(x, y)

# Return multiple values
def min_max(nums):
    return min(nums), max(nums)

print(min_max([1,5,9]))
```

---

## **8. Sets**

```python
items = {"apple", "banana", "apple"}  # unique
items.add("orange")
items.remove("banana")

# Operations
a = {1,2,3}
b = {3,4,5}
print(a | b)   # union
print(a & b)   # intersection
print(a - b)   # difference
print(a ^ b)   # symmetric difference

# Frozen set
fset = frozenset([1,2,3])
```

---

## **9. Dictionaries**

```python
product = {"name": "Laptop", "price": 45000}

# Access
print(product["name"])
print(product.get("price"))

# Methods
print(product.keys())
print(product.values())
print(product.items())

product.update({"stock": 50})
copy = product.copy()

# Comprehension
squares = {x: x*x for x in range(5)}

# Nested
users = {
    "alice": {"age": 25, "city": "NY"},
    "bob": {"age": 30, "city": "LA"}
}
```

---

## **10. Numbers & Math**

```python
# Built-in
print(round(4.7))
print(abs(-5))
print(pow(2,3))
print(divmod(9,2))

# Math module
import math
print(math.pi)
print(math.sqrt(16))
print(math.sin(math.radians(30)))

# Random
import random
print(random.random())
print(random.choice([1,2,3]))
print(random.sample([1,2,3,4], 2))
random.shuffle([1,2,3,4])
```

---

## **11. Dates & Time**

```python
from datetime import datetime, timedelta

# Now
now = datetime.now()
print(now)

# Create
birthday = datetime(1990, 5, 21)

# Extract
print(now.day, now.month, now.year, now.weekday())

# Format
print(now.strftime("%d-%m-%Y %H:%M:%S"))

# Difference
diff = now - birthday
print(diff.days)
```

---

## **12. Classes & OOP**

```python
class Employee:
    company = "TechCorp"   # class variable
    
    def __init__(self, name, role):
        self.name = name
        self.role = role
    
    def get_details(self):   # instance method
        return f"{self.name} works as a {self.role}"
    
    @classmethod
    def set_company(cls, company):
        cls.company = company
    
    @staticmethod
    def greet():
        return "Welcome to TechCorp!"
    
    def __str__(self): return f"Employee: {self.name}"
    def __eq__(self, other): return self.name == other.name

class Manager(Employee):    # inheritance
    def get_details(self):
        return f"{self.name} manages a team"

e1 = Employee("John", "Developer")
m1 = Manager("Alice", "Manager")
```

---

## **13. File Handling**

```python
# Opening & Reading
with open("data.txt", "w") as f:
    f.write("Hello World")

with open("data.txt", "r") as f:
    print(f.read())

# Append
with open("data.txt", "a") as f:
    f.write("\nNew line added")

# JSON
import json
data = {"product": "Laptop", "price": 45000}
with open("data.json", "w") as f: json.dump(data, f)
with open("data.json", "r") as f: print(json.load(f))

# os operations
import os
os.rename("data.txt", "info.txt")
print(os.path.exists("info.txt"))
os.remove("info.txt")
```