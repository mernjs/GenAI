# **Node.js for Beginners**

---

## **1. Variables & Data Types**

### **var, let, const**

```js
var companyName = "TechCorp";         // Old style (avoid)
let employeeCount = 120;              // Can be reassigned
const foundedYear = 2010;             // Constant value
```

### **Primitive Types**

```js
const productName = "Laptop";          // string
const price = 45000;                   // number
const isAvailable = true;              // boolean
let discount;                          // undefined
const warranty = null;                 // null
const uniqueID = Symbol("id");         // symbol
const bigRevenue = 1234567890123n;     // bigint
```

### **Reference Types**

```js
const product = { name: "Mouse", price: 499 };   // object
const categories = ["Electronics", "Clothing"];  // array
function calculateGST(amount) { return amount * 0.18; } // function
```

---

## **2. Operators**

### **Arithmetic**

```js
let revenue = 10000;
let expenses = 4000;
let profit = revenue - expenses;  // 6000
```

### **Assignment**

```js
profit += 500;  // Adds bonus → 6500
```

### **Comparison**

```js
console.log(profit > 5000);  // true
```

### **Logical**

```js
const hasStock = true;
const isOnline = false;
console.log(hasStock && isOnline);  // false
```

### **Ternary**

```js
const status = profit > 5000 ? "High Profit" : "Low Profit";
console.log(status);  // "High Profit"
```

---

## **3. Control Structures**

### **if-else**

```js
let rating = 4.5;
if (rating >= 4.5) {
  console.log("Excellent product");
} else {
  console.log("Average product");
}
```

### **switch**

```js
let paymentMethod = "UPI";
switch (paymentMethod) {
  case "Credit Card": console.log("Processing via Credit Card"); break;
  case "UPI": console.log("Processing via UPI"); break;
  default: console.log("Payment method not supported");
}
```

### **Loops**

```js
const products = ["Laptop", "Phone", "Tablet"];

// for loop
for (let i = 0; i < products.length; i++) console.log(products[i]);

// while loop
let i = 0;
while (i < 2) { console.log("Offer available"); i++; }

// do...while
let j = 0;
do { console.log("Limited stock"); j++; } while (j < 1);

// for...of
for (let item of products) console.log(item);

// for...in
for (let index in products) console.log(index, products[index]);
```

---

## **4. Functions**

### **Function Declaration**

```js
function greetCustomer(name) {
  return `Hello ${name}, welcome to TechStore!`;
}
```

### **Function Expression**

```js
const addToCart = function(product) {
  return `${product} added to your cart.`;
};
```

### **Arrow Function**

```js
const calculateDiscount = (price, discount = 10) => price - (price * discount) / 100;
```

### **Default Parameters**

```js
function shippingCharge(location = "India") {
  return location === "India" ? 50 : 200;
}
```

### **Rest & Spread**

```js
function orderSummary(...items) {
  return `You ordered: ${items.join(", ")}`;
}
const order = ["Laptop", "Mouse"];
console.log(orderSummary(...order));
```

### **Higher Order Functions**

```js
const prices = [100, 200, 300];

const discounted = prices.map(p => p * 0.9);        // map
const expensive = prices.filter(p => p > 150);      // filter
const total = prices.reduce((sum, p) => sum + p, 0); // reduce
```

---

## **5. Strings**

```js
const customer = "   Alice Johnson   ";

// Properties
console.log(customer.length); 
console.log(customer.charAt(2)); 
console.log(customer.indexOf("J")); 
console.log(customer.includes("Alice")); 

// Manipulation
console.log(customer.slice(3, 8)); 
console.log(customer.replace("Alice", "Bob")); 
console.log(customer.toUpperCase()); 
console.log(customer.trim()); 

// Template literal
let orderId = 101;
console.log(`Order ID: ${orderId} for customer ${customer.trim()}`);

// Split, Join, Concat
const skills = "JS,Node,React".split(",");
console.log(skills.join(" | "));
console.log("Hello".concat(" World"));
```

---

## **6. Arrays**

```js
const cart = ["Laptop", "Phone"];

// Add/Remove
cart.push("Mouse"); 
cart.pop();
cart.shift();
cart.unshift("Tablet");

// Search
console.log(cart.indexOf("Phone"));
console.log(cart.includes("Laptop"));
console.log(cart.find(item => item === "Laptop"));
console.log(cart.findIndex(item => item === "Phone"));

// Transform
const prices = [100, 200, 300];
console.log(prices.map(p => p * 2));
console.log(prices.filter(p => p > 150));
console.log(prices.reduce((a, b) => a + b));
console.log(prices.sort());
console.log(prices.reverse());

// Combine
const electronics = ["TV", "Fridge"];
const appliances = ["Mixer", "Grinder"];
console.log(electronics.concat(appliances));
console.log(electronics.slice(0, 1));
electronics.splice(1, 0, "AC"); 
```

---

## **7. Numbers & Math**

```js
let price = 1234.567;
console.log(price.toFixed(2));
console.log(price.toPrecision(5));
console.log(Number.isNaN(NaN));
console.log(Number.isInteger(100));

// Math
console.log(Math.PI);
console.log(Math.round(4.7));
console.log(Math.floor(4.9));
console.log(Math.ceil(4.1));
console.log(Math.trunc(4.9));
console.log(Math.random());
console.log(Math.pow(2, 3));
console.log(Math.sqrt(16));
console.log(Math.abs(-5));
console.log(Math.max(10, 20));
```

---

## **8. Dates**

```js
let today = new Date();
console.log(today);

// Getters
console.log(today.getDate());
console.log(today.getMonth() + 1); 
console.log(today.getFullYear());
console.log(today.getDay());
console.log(today.getHours());

// Setters
today.setDate(15);
today.setMonth(11);
today.setFullYear(2025);

// Formatting
console.log(today.toDateString());
console.log(today.toISOString());
```

---

## **9. Objects**

```js
const product = {
  name: "Laptop",
  price: 45000,
  showDetails() {
    console.log(`Product: ${this.name}, Price: ₹${this.price}`);
  }
};

// Access
console.log(product.name);
console.log(product["price"]);
product.showDetails();

// Object methods
console.log(Object.keys(product));
console.log(Object.values(product));
console.log(Object.entries(product));
Object.freeze(product);

// Destructuring
const { name, price } = product;
console.log(name, price);
```

---

## **10. Classes**

```js
class Employee {
  constructor(name, role) {
    this.name = name;
    this.role = role;
  }
  getDetails() {
    return `${this.name} works as a ${this.role}`;
  }
}

const emp = new Employee("John", "Developer");
console.log(emp.getDetails());
```

---

## **11. File Handling (fs module in Node.js)**

```js
const fs = require("fs");

// Write
fs.writeFileSync("data.json", JSON.stringify({ product: "Laptop", price: 45000 }));

// Read
const data = fs.readFileSync("data.json", "utf-8");
console.log("File Content:", data);

// Append
fs.appendFileSync("data.json", "\nNew entry added");

// Rename
fs.renameSync("data.json", "products.json");

// Delete
fs.unlinkSync("products.json");
```