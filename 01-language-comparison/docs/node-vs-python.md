# Node.js vs Python – Beginner’s Comparison

## **1. Variables & Data Types**

**Definition:**

* **Node.js (JavaScript):** Variables can be declared using `var`, `let`, or `const`. It supports primitive types (string, number, boolean, null, undefined, symbol, bigint) and reference types (object, array, function).
* **Python:** Variables are dynamically typed, declared by assignment. It supports primitive types (`str`, `int`, `float`, `bool`, `None`, `complex`) and reference types (`list`, `tuple`, `dict`, `set`, function, object).

**Example:**

```js
// Node.js
let companyName = "TechCorp"; 
const foundedYear = 2010;     
let isAvailable = true;       
let discount = null;          
let bigRevenue = 1234567890123n; 
```

```python
# Python
company_name = "TechCorp"   
founded_year = 2010         
is_available = True         
discount = None             
big_revenue = 1234567890123 
```

---

## **2. Operators**

**Definition:**

* **Node.js:** Supports arithmetic, assignment, comparison, logical, and ternary operators.
* **Python:** Similar operators, with additional `is` (identity) and `in` (membership).

**Example:**

```js
// Node.js
let profit = 10000 - 4000;
profit += 500;           
let status = profit > 5000 ? "High" : "Low";
```

```python
# Python
profit = 10000 - 4000
profit += 500
status = "High" if profit > 5000 else "Low"
```

---

## **3. Control Structures**

**Definition:**

* **Node.js:** Uses `if`, `else`, `switch`, and loop constructs (`for`, `while`, `for...of`, `for...in`).
* **Python:** Uses `if`, `elif`, `else`, `match case` (like `switch`), and loops (`for`, `while`).

**Example:**

```js
// Node.js
if (rating >= 4.5) console.log("Excellent");
else console.log("Average");

switch(paymentMethod) {
  case "UPI": console.log("UPI"); break;
  default: console.log("Other");
}
```

```python
# Python
if rating >= 4.5:
    print("Excellent")
else:
    print("Average")

match payment_method:
    case "UPI":
        print("UPI")
    case _:
        print("Other")
```

---

## **4. Functions**

**Definition:**

* **Node.js:** Functions can be declared, expressed, or written as arrow functions. Supports default parameters, rest/spread, higher-order functions.
* **Python:** Functions are defined with `def`, support default parameters, `*args`, `**kwargs`, lambdas, recursion, and higher-order functions.

**Example:**

```js
// Node.js
function greet(name) {
  return `Hello ${name}`;
}
const discount = (price, rate=10) => price - (price*rate)/100;
```

```python
# Python
def greet(name):
    return f"Hello {name}"

discount = lambda price, rate=10: price - (price*rate)/100
```

---

## **5. Strings**

**Definition:**

* **Node.js:** Strings are immutable, with methods like `.slice()`, `.replace()`, `.toUpperCase()`. Template literals (`${}`) allow interpolation.
* **Python:** Strings are immutable with rich methods (`.upper()`, `.strip()`, `.replace()`). Supports f-strings, `.format()`, `%` formatting.

**Example:**

```js
// Node.js
let name = " Alice ";
console.log(name.trim().toUpperCase());
console.log(`Welcome, ${name.trim()}`);
```

```python
# Python
name = " Alice "
print(name.strip().upper())
print(f"Welcome, {name.strip()}")
```

---

## **6. Arrays vs Lists**

**Definition:**

* **Node.js:** Arrays are ordered, mutable collections.
* **Python:** Lists are ordered, mutable collections with similar methods.

**Example:**

```js
// Node.js
let cart = ["Laptop", "Phone"];
cart.push("Mouse");
console.log(cart.includes("Laptop"));
```

```python
# Python
cart = ["Laptop", "Phone"]
cart.append("Mouse")
print("Laptop" in cart)
```

---

## **7. Tuples**

**Definition:**

* **Node.js:** No native tuple, arrays are often used instead.
* **Python:** Tuples are immutable ordered collections, useful for fixed data.

**Example:**

```python
# Python
coords = (10, 20)
x, y = coords
```

---

## **8. Sets**

**Definition:**

* **Node.js:** `Set` stores unique values.
* **Python:** `set` stores unique values, supports mathematical set operations.

**Example:**

```js
// Node.js
let items = new Set(["apple", "banana"]);
items.add("orange");
```

```python
# Python
items = {"apple", "banana"}
items.add("orange")
```

---

## **9. Dictionaries vs Objects**

**Definition:**

* **Node.js:** Objects are key-value pairs `{key: value}`.
* **Python:** Dictionaries are key-value pairs with rich methods.

**Example:**

```js
// Node.js
let product = { name: "Laptop", price: 45000 };
console.log(product.name);
```

```python
# Python
product = {"name": "Laptop", "price": 45000}
print(product["name"])
```

---

## **10. Numbers & Math**

**Definition:**

* **Node.js:** `Math` object for math operations.
* **Python:** `math` and `random` modules for math and randomness.

**Example:**

```js
// Node.js
console.log(Math.PI);
console.log(Math.sqrt(16));
console.log(Math.random());
```

```python
# Python
import math, random
print(math.pi)
print(math.sqrt(16))
print(random.random())
```

---

## **11. Dates & Time**

**Definition:**

* **Node.js:** `Date` object for date/time handling.
* **Python:** `datetime` module for powerful date/time manipulation.

**Example:**

```js
// Node.js
let today = new Date();
console.log(today.toISOString());
```

```python
# Python
from datetime import datetime
today = datetime.now()
print(today.isoformat())
```

---

## **12. Classes & OOP**

**Definition:**

* **Node.js:** Uses `class`, `constructor`, methods, inheritance.
* **Python:** Similar OOP support with `class`, `__init__`, methods, inheritance, encapsulation.

**Example:**

```js
// Node.js
class Employee {
  constructor(name) { this.name = name; }
  getDetails() { return `Employee: ${this.name}`; }
}
```

```python
# Python
class Employee:
    def __init__(self, name):
        self.name = name
    def get_details(self):
        return f"Employee: {self.name}"
```

---

## **13. File Handling**

**Definition:**

* **Node.js:** Uses `fs` module for reading/writing files.
* **Python:** Uses built-in `open()` and `with` context manager.

**Example:**

```js
// Node.js
const fs = require("fs");
fs.writeFileSync("data.txt", "Hello World");
let data = fs.readFileSync("data.txt", "utf-8");
```

```python
# Python
with open("data.txt", "w") as f:
    f.write("Hello World")

with open("data.txt", "r") as f:
    data = f.read()
```