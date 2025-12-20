# Node.js vs Python – Complete Beginner to Intermediate README

This README is designed for **absolute beginners** who want to understand **Node.js and Python side-by-side** and for **developers** who want a **clear comparison** before choosing a backend stack.

It explains:

* Core language concepts
* Syntax differences
* Practical examples
* Performance and scalability
* Frameworks
* Real-world use cases
* Career and job market impact

---

## 1. What Are Node.js and Python?

### Node.js

Node.js is a **runtime environment** that allows JavaScript to run **outside the browser**, mainly on servers.

* Uses **JavaScript**
* Built on **Chrome’s V8 engine**
* Designed for **event-driven, non-blocking I/O**
* Excellent for **real-time and high-concurrency applications**

### Python

Python is a **general-purpose programming language** known for its **simplicity and readability**.

* Clean and beginner-friendly syntax
* Strong support for **web, data, AI, automation**
* Huge ecosystem of libraries
* Very popular in **backend, AI, and enterprise systems**

---

# **Node.js vs Python - Comparison**

| **Feature / Purpose**            | **Node.js**                                 | **Python**                               |
| -------------------------------- | ------------------------------------------- | ---------------------------------------- |
| **Language Runtime**             | `node`                                      | `python`                                 |
| **Install (System-level)**       | Download [nodejs.org](https://nodejs.org)   | Download [python.org](https://python.org)|
| **Primary Language**             | JavaScript / TypeScript                     | Python                                   |
| **Typing System**                | Static (TypeScript)                         | Dynamic (Optional typing)                |
| **Async Support**                | Native & default                            | Supported, not default                   |
| **Event Loop**                   | Built-in, core to runtime                   | Abstracted                               |
| **Package Manager**              | `npm`,  `yarn`                              | `pip`                                    |
| **Init New Project**             | `npm init`                                  | Manual                                   |
| **Install Package (Local)**      | `npm install express prisma @prisma/client` | `pip install fastapi uvicorn sqlalchemy` |
| **Install Package (Global)**     | `npm install -g nodemon`                    | `pip install --user uvicorn`             |
| **Version Manager**              | `nvm`                                       | `pyenv`                                  |
| **Environment Management**       | `.nvmrc`                                    | `venv`, `.python-version`                |
| **Create Virtual Environment**   | Not required                                | `python -m venv env`                     |
| **Activate Virtual Environment** | N/A                                         | `source env/bin/activate`                |
| **Dependency Lock File**         | `package-lock.json`, `yarn.lock`            | `requirements.txt`,                      |
| **Script Runner**                | `package.json` scripts                      | `Makefile`, `invoke`, `tox`              |
| **Development Server**           | `node index.js`, `nodemon`                  | `uvicorn main:app --reload`              |
| **Framework (API)**              | Express / Fastify / NestJS                  | FastAPI / Flask / Django                 |
| **Routing Style**                | Callback / middleware based                 | Decorator based                          |
| **Request Validation**           | External libs (Zod, Joi)                    | Built-in (Pydantic)                      |
| **Error Handling**               | Manual `try/catch`                          | Exception based                          |
| **Middleware Pattern**           | Chain-based                                 | Dependency Injection                     |
| **Database ORM / Client**        | Prisma                                      | SQLAlchemy                               |
| **Schema Definition**            | Centralized schema file                     | Distributed models                       |
| **Type-safe DB Queries**         | Yes                                         | Partial                                  |
| **Raw SQL Support**              | Yes                                         | Yes                                      |
| **OAuth / SSO**                  | Strong ecosystem                            | Stable ecosystem                         |
| **Background Jobs**              | BullMQ                                      | Celery                                   |
| **Async Job Workers**            | Native                                      | Requires config                          |
| **Testing Framework**            | Jest / Vitest                               | Pytest                                   |
| **Mocking Support**              | Easy                                        | Very powerful                            |
| **Logging Libraries**            | Winston, Pino                               | logging, loguru                          |
| **CLI Tooling**                  | Excellent                                   | Excellent                                |
| **Monorepo Support**             | Excellent                                   | Limited                                  |
| **CPU-bound Tasks**              | Worker Threads                              | Multiprocessing                          |
| **Memory Usage**                 | Low                                         | Medium                                   |
| **Startup Time**                 | Fast                                        | Moderate                                 |
| **Serverless Support**           | Excellent                                   | Good                                     |
| **Docker Image Size**            | Smaller                                     | Larger                                   |
| **Large Codebase Handling**      | Excellent                                   | Requires discipline                      |
| **Frontend Type Sharing**        | Easy                                        | Not possible                             |
| **AI / ML Integration**          | Weak                                        | Excellent                                |
| **Official Registry**            | npmjs.com                                   | pypi.org                                 |


---

| **Feature / Purpose**       | **Node.js**          | **Python**         |
| --------------------------- | -------------------- | ------------------ |
| **Web Framework (Minimal)** | `express`            | `flask`            |
| **Web Framework (Modern)**  | `fastify`            | `fastapi`          |
| **Enterprise Framework**    | `nestjs`             | `django`           |
| **Async-first Framework**   | `fastify`            | `fastapi`          |
| **Validation Library**      | `zod`                | `pydantic`         |
| **Form/Data Parsing**       | `body-parser`        | Built-in           |
| **OpenAPI Generation**      | `swagger-jsdoc`      | Built-in (FastAPI) |
| **Primary ORM**             | `prisma`             | `sqlalchemy`       |
| **NoSQL (MongoDB)**         | `mongoose`           | `mongoengine`      |
| **Password Hashing**        | `bcryptjs`           | `bcrypt`           |
| **JWT**                     | `jsonwebtoken`       | `pyjwt`            |
| **OAuth / SSO**             | `passport`           | `authlib`          |
| **Rate Limiting**           | `express-rate-limit` | `slowapi`          |
| **CORS**                    | `cors`               | `fastapi-cors`     |
| **Test Runner**             | `jest`               | `pytest`           |
| **Error Tracking**          | `sentry`             | `sentry-sdk`       |
| **Structured Logging**      | `pino`               | `loguru`           |
| **Default Logging**         | `winston`            | `logging`          |
| **Env Loader**              | `dotenv`             | `python-dotenv`    |
| **Job Queue**               | `bullmq`             | `celery`           |
| **Redis-based Queue**       | `bull`               | `rq`               |
| **Scheduler**               | `node-cron`          | `apscheduler`      |
| **Worker Management**       | Built-in             | External           |
| **HTTP Client**             | `axios`              | `requests`         |
| **File Upload**             | `multer`             | `python-multipart` |
| **AWS S3**                  | `aws-sdk`            | `boto3`            |
| **WebSockets**              | `socket.io`          | `websockets`       |
| **In-memory Cache**         | `node-cache`         | `cachetools`       |
| **Redis Cache**             | `ioredis`            | `redis-py`         |
| **Dev Server Reload**       | `nodemon`            | `uvicorn --reload` |
| **Formatting**              | `prettier`           | `black`            |


# Core 
## 2. Variables and Data Types

### Node.js (JavaScript)

* Variables declared using `var`, `let`, or `const`
* Dynamically typed
* Supports primitive and reference types

```js
let companyName = "TechCorp";
const foundedYear = 2010;
let isAvailable = true;
let discount = null;
let bigRevenue = 1234567890123n;
```

**Primitive Types**

* string
* number
* boolean
* null
* undefined
* symbol
* bigint

**Reference Types**

* object
* array
* function

---

### Python

* Variables created by assignment
* Dynamically typed
* Cleaner naming conventions

```python
company_name = "TechCorp"
founded_year = 2010
is_available = True
discount = None
big_revenue = 1234567890123
```

**Primitive Types**

* str
* int
* float
* bool
* None
* complex

**Reference Types**

* list
* tuple
* dict
* set
* function
* object

---

## 3. Operators

### Node.js

```js
let profit = 10000 - 4000;
profit += 500;
let status = profit > 5000 ? "High" : "Low";
```

Supports:

* Arithmetic
* Assignment
* Comparison
* Logical
* Ternary

---

### Python

```python
profit = 10000 - 4000
profit += 500
status = "High" if profit > 5000 else "Low"
```

Extra operators:

* `in` → membership
* `is` → identity

---

## 4. Control Structures

### Node.js

```js
if (rating >= 4.5) {
  console.log("Excellent");
} else {
  console.log("Average");
}

switch(paymentMethod) {
  case "UPI":
    console.log("UPI");
    break;
  default:
    console.log("Other");
}
```

Loops:

* for
* while
* do...while
* for...of
* for...in

---

### Python

```python
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

Loops:

* for
* while
* range
* enumerate
* zip

---

## 5. Functions

### Node.js

```js
function greet(name) {
  return `Hello ${name}`;
}

const discount = (price, rate = 10) =>
  price - (price * rate) / 100;
```

Supports:

* Function declaration
* Function expression
* Arrow functions
* Default parameters
* Rest and spread
* Higher-order functions

---

### Python

```python
def greet(name):
    return f"Hello {name}"

discount = lambda price, rate=10: price - (price * rate) / 100
```

Supports:

* def functions
* lambda
* *args and **kwargs
* recursion
* decorators
* higher-order functions

---

## 6. Strings

### Node.js

```js
let name = " Alice ";
console.log(name.trim().toUpperCase());
console.log(`Welcome, ${name.trim()}`);
```

Key points:

* Immutable
* Template literals for interpolation

---

### Python

```python
name = " Alice "
print(name.strip().upper())
print(f"Welcome, {name.strip()}")
```

Supports:

* f-strings
* format()
* % formatting

---

## 7. Arrays vs Lists

### Node.js Arrays

```js
let cart = ["Laptop", "Phone"];
cart.push("Mouse");
console.log(cart.includes("Laptop"));
```

---

### Python Lists

```python
cart = ["Laptop", "Phone"]
cart.append("Mouse")
print("Laptop" in cart)
```

---

## 8. Tuples

* Node.js has no native tuple
* Python tuples are immutable

```python
coords = (10, 20)
x, y = coords
```

---

## 9. Sets

### Node.js

```js
let items = new Set(["apple", "banana"]);
items.add("orange");
```

---

### Python

```python
items = {"apple", "banana"}
items.add("orange")
```

Python supports:

* union
* intersection
* difference

---

## 10. Objects vs Dictionaries

### Node.js Objects

```js
let product = { name: "Laptop", price: 45000 };
console.log(product.name);
```

---

### Python Dictionaries

```python
product = {"name": "Laptop", "price": 45000}
print(product["name"])
```

---

## 11. Numbers and Math

### Node.js

```js
console.log(Math.PI);
console.log(Math.sqrt(16));
console.log(Math.random());
```

---

### Python

```python
import math, random
print(math.pi)
print(math.sqrt(16))
print(random.random())
```

---

## 12. Dates and Time

### Node.js

```js
let today = new Date();
console.log(today.toISOString());
```

---

### Python

```python
from datetime import datetime
today = datetime.now()
print(today.isoformat())
```

---

## 13. Classes and OOP

### Node.js

```js
class Employee {
  constructor(name) {
    this.name = name;
  }
  getDetails() {
    return `Employee: ${this.name}`;
  }
}
```

---

### Python

```python
class Employee:
    def __init__(self, name):
        self.name = name
    def get_details(self):
        return f"Employee: {self.name}"
```

Python also supports:

* inheritance
* static methods
* class methods
* magic methods

---

## 14. File Handling

### Node.js

```js
const fs = require("fs");
fs.writeFileSync("data.txt", "Hello World");
let data = fs.readFileSync("data.txt", "utf-8");
```

---

### Python

```python
with open("data.txt", "w") as f:
    f.write("Hello World")

with open("data.txt", "r") as f:
    data = f.read()
```

---

### **1. Web Framework (Minimal)**

#### Definition

* **Node.js:** Minimal HTTP server using Express
* **Python:** Minimal HTTP server using Flask

#### Example

```js
// Node.js - Express
const express = require("express");
const app = express();

app.get("/", (req, res) => {
  res.json({ message: "Hello from Express" });
});

app.listen(3000, () => console.log("Server running on port 3000"));
```

```python
# Python - Flask
from flask import Flask, jsonify

app = Flask(__name__)

@app.route("/")
def home():
    return jsonify(message="Hello from Flask")

app.run(port=3000)
```

---

### **2. Web Framework (Modern / Async-first)**

#### Definition

* **Node.js:** Fastify (async-first, high performance)
* **Python:** FastAPI (async-first, type-based)

#### Example

```js
// Node.js - Fastify
const fastify = require("fastify")();

fastify.get("/", async () => {
  return { message: "Hello from Fastify" };
});

fastify.listen({ port: 3000 });
```

```python
# Python - FastAPI
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
async def home():
    return {"message": "Hello from FastAPI"}
```

---

### **3. Enterprise Framework**

#### Definition

* **Node.js:** NestJS (opinionated, modular)
* **Python:** Django (batteries included)

#### Example

```ts
// Node.js - NestJS Controller
import { Controller, Get } from "@nestjs/common";

@Controller()
export class AppController {
  @Get()
  getHello() {
    return { message: "Hello from NestJS" };
  }
}
```

```python
# Python - Django View
from django.http import JsonResponse

def home(request):
    return JsonResponse({"message": "Hello from Django"})
```

---

### **4. Routing Style**

#### Definition

* **Node.js:** Middleware & callback based
* **Python:** Decorator based

#### Example

```js
// Node.js
app.get("/users", (req, res) => {
  res.send("Users list");
});
```

```python
# Python
@app.get("/users")
def users():
    return "Users list"
```

---

### **5. Request Validation**

#### Definition

* **Node.js:** External validation libraries
* **Python:** Built-in with FastAPI + Pydantic

#### Example

```ts
// Node.js - Zod
import { z } from "zod";

const schema = z.object({
  email: z.string().email(),
});

schema.parse({ email: "test@example.com" });
```

```python
# Python - Pydantic
from pydantic import BaseModel

class User(BaseModel):
    email: str
```

---

### **6. ORM / Database Access**

#### Definition

* **Node.js:** Prisma (type-safe ORM)
* **Python:** SQLAlchemy (flexible ORM)

#### Example

```ts
// Node.js - Prisma
const user = await prisma.user.create({
  data: { email: "test@example.com" },
});
```

```python
# Python - SQLAlchemy
user = User(email="test@example.com")
session.add(user)
session.commit()
```

---

### **7. Authentication (JWT)**

#### Definition

* **Node.js:** jsonwebtoken
* **Python:** pyjwt

#### Example

```js
// Node.js
const jwt = require("jsonwebtoken");

const token = jwt.sign({ userId: 1 }, "secret");
```

```python
# Python
import jwt

token = jwt.encode({"userId": 1}, "secret", algorithm="HS256")
```

---

### **8. Background Jobs**

#### Definition

* **Node.js:** BullMQ (Redis-based)
* **Python:** Celery

#### Example

```js
// Node.js - BullMQ
import { Queue } from "bullmq";

const queue = new Queue("emails");
queue.add("sendEmail", { to: "user@test.com" });
```

```python
# Python - Celery
from celery import Celery

app = Celery("tasks", broker="redis://localhost")

@app.task
def send_email(to):
    print("Sending email to", to)
```

---

### **9. Testing**

#### Definition

* **Node.js:** Jest
* **Python:** Pytest

#### Example

```js
// Node.js - Jest
test("sum", () => {
  expect(1 + 2).toBe(3);
});
```

```python
# Python - Pytest
def test_sum():
    assert 1 + 2 == 3
```

---

### **10. WebSockets**

#### Definition

* **Node.js:** socket.io
* **Python:** websockets

#### Example

```js
// Node.js - socket.io
io.on("connection", socket => {
  socket.emit("message", "Hello client");
});
```

```python
# Python - websockets
async def handler(ws):
    await ws.send("Hello client")
```

---

### **11. Logging**

#### Definition

* **Node.js:** Pino / Winston
* **Python:** logging / loguru

#### Example

```js
// Node.js
const logger = require("pino")();
logger.info("App started");
```

```python
# Python
import logging
logging.info("App started")
```

---

### **12. Environment Variables**

#### Definition

* **Node.js:** dotenv
* **Python:** python-dotenv

#### Example

```js
// Node.js
require("dotenv").config();
console.log(process.env.DB_URL);
```

```python
# Python
from dotenv import load_dotenv
load_dotenv()
```

---

### **13. Middleware Pattern**

#### Definition

* **Node.js:** Chain-based middleware execution
* **Python:** Dependency Injection (FastAPI)

#### Example

```js
// Node.js - Express Middleware
function auth(req, res, next) {
  if (!req.headers.authorization) {
    return res.status(401).send("Unauthorized");
  }
  next();
}

app.get("/secure", auth, (req, res) => {
  res.send("Secure data");
});
```

```python
# Python - FastAPI Dependency
from fastapi import Depends, HTTPException

def auth(token: str = ""):
    if not token:
        raise HTTPException(status_code=401)

@app.get("/secure")
def secure(dep=Depends(auth)):
    return "Secure data"
```

---

### **14. Error Handling**

#### Definition

* **Node.js:** Manual try/catch
* **Python:** Exception-based handling

#### Example

```js
// Node.js
app.get("/error", async (req, res) => {
  try {
    throw new Error("Something failed");
  } catch (err) {
    res.status(500).json({ error: err.message });
  }
});
```

```python
# Python
@app.get("/error")
def error():
    raise Exception("Something failed")
```

---

### **15. Database Migration**

#### Definition

* **Node.js:** Prisma migrate
* **Python:** Alembic

#### Example

```bash
# Node.js
npx prisma migrate dev --name init
```

```bash
# Python
alembic revision --autogenerate -m "init"
alembic upgrade head
```

---

### **16. Type-safe Database Queries**

#### Definition

* **Node.js:** Fully type-safe (Prisma + TS)
* **Python:** Partially type-safe

#### Example

```ts
// Node.js
const user = await prisma.user.findUnique({
  where: { id: 1 },
});
```

```python
# Python
user = session.query(User).filter(User.id == 1).first()
```

---

### **17. Raw SQL Execution**

#### Definition

* **Node.js:** Supported via ORM
* **Python:** Supported via ORM

#### Example

```ts
// Node.js
await prisma.$queryRaw`SELECT * FROM users`;
```

```python
# Python
session.execute("SELECT * FROM users")
```

---

### **18. Password Hashing**

#### Definition

* **Node.js:** bcryptjs / argon2
* **Python:** bcrypt / passlib

#### Example

```js
// Node.js
const bcrypt = require("bcryptjs");
const hash = await bcrypt.hash("password", 10);
```

```python
# Python
import bcrypt
hashed = bcrypt.hashpw(b"password", bcrypt.gensalt())
```

---

### **19. OAuth / SSO**

#### Definition

* **Node.js:** Passport
* **Python:** Authlib

#### Example

```js
// Node.js - Passport Strategy
passport.use(new GoogleStrategy({
  clientID: "id",
  clientSecret: "secret",
}, verifyFn));
```

```python
# Python - Authlib
oauth.register(
    name="google",
    client_id="id",
    client_secret="secret"
)
```

---

### **20. Async Job Workers**

#### Definition

* **Node.js:** Native async workers
* **Python:** Requires explicit worker setup

#### Example

```js
// Node.js
async function worker(job) {
  await process(job);
}
```

```python
# Python
@app.task
def worker(job):
    process(job)
```

---

### **22. CLI Tooling**

#### Definition

* **Node.js:** Native CLI scripts
* **Python:** argparse / click

#### Example

```js
// Node.js
#!/usr/bin/env node
console.log("CLI tool");
```

```python
# Python
import argparse
parser = argparse.ArgumentParser()
parser.parse_args()
```

---

### **23. CPU-bound Tasks**

#### Definition

* **Node.js:** Worker Threads
* **Python:** Multiprocessing

#### Example

```js
// Node.js
const { Worker } = require("worker_threads");
new Worker("./task.js");
```

```python
# Python
from multiprocessing import Process
Process(target=task).start()
```

---

### **24. Serverless Support**

#### Definition

* **Node.js:** Excellent support
* **Python:** Good support

#### Example

```js
// Node.js - AWS Lambda
exports.handler = async () => ({
  statusCode: 200,
  body: "Hello",
});
```

```python
# Python - AWS Lambda
def handler(event, context):
    return {"statusCode": 200, "body": "Hello"}
```

---

### **25. Dockerization**

#### Definition

* **Node.js:** Smaller images
* **Python:** Larger images

#### Example

```dockerfile
# Node.js
FROM node:20-alpine
WORKDIR /app
COPY . .
CMD ["node", "index.js"]
```

```dockerfile
# Python
FROM python:3.12-slim
WORKDIR /app
COPY . .
CMD ["python", "main.py"]
```

---

### **26. Frontend Type Sharing**

#### Definition

* **Node.js:** Shared TypeScript types
* **Python:** Not possible

#### Example

```ts
// Shared type
export interface User {
  id: number;
  email: string;
}
```

```python
# Python (no direct sharing)
class User(BaseModel):
    id: int
```

---

### **27. AI / ML Integration**

#### Definition

* **Node.js:** Weak ecosystem
* **Python:** Excellent ecosystem

#### Example

```js
// Node.js
const response = await openai.responses.create({...});
```

```python
# Python
import torch
model = torch.load("model.pt")
```

---

### **29. Startup Time**

#### Definition

* **Node.js:** Fast
* **Python:** Moderate

#### Example

```js
console.time("start");
```

```python
import time; start = time.time()
```

---

### **30. Official Package Registry**

#### Definition

* **Node.js:** npm
* **Python:** PyPI

#### Example

```bash
# Node.js
npm publish
```

```bash
# Python
pip install mypackage
```

### **FILE 1 — Node.js (index.js)**

**Tech used:** Express + Prisma + JWT + Zod + Socket.IO

#### Install dependencies

```bash
npm init -y
npm install express zod jsonwebtoken bcryptjs prisma @prisma/client socket.io dotenv
```

```bash
npx prisma init
```

**prisma/schema.prisma**

```prisma
datasource db {
  provider = "sqlite"
  url      = "file:./dev.db"
}

generator client {
  provider = "prisma-client-js"
}

model User {
  id       Int     @id @default(autoincrement())
  email    String  @unique
  password String
}
```

```bash
npx prisma migrate dev --name init
```

---

###### **index.js (FULL WORKING CODE)**

```js
require("dotenv").config();
const express = require("express");
const http = require("http");
const jwt = require("jsonwebtoken");
const bcrypt = require("bcryptjs");
const { z } = require("zod");
const { PrismaClient } = require("@prisma/client");
const { Server } = require("socket.io");

const app = express();
const server = http.createServer(app);
const io = new Server(server);

const prisma = new PrismaClient();
app.use(express.json());

/* ---------- LOGGER MIDDLEWARE ---------- */
app.use((req, res, next) => {
  console.log(`[NODE] ${req.method} ${req.url}`);
  next();
});

/* ---------- AUTH MIDDLEWARE ---------- */
function auth(req, res, next) {
  try {
    const token = req.headers.authorization?.split(" ")[1];
    req.user = jwt.verify(token, "secret");
    next();
  } catch {
    res.status(401).json({ error: "Unauthorized" });
  }
}

/* ---------- VALIDATION ---------- */
const userSchema = z.object({
  email: z.string().email(),
  password: z.string().min(6),
});

/* ---------- ROUTES ---------- */

// Health
app.get("/", (_, res) => {
  res.json({ status: "Node API Running" });
});

// Register
app.post("/register", async (req, res) => {
  const body = userSchema.parse(req.body);
  const hash = await bcrypt.hash(body.password, 10);

  const user = await prisma.user.create({
    data: { email: body.email, password: hash },
  });

  res.json(user);
});

// Login
app.post("/login", async (req, res) => {
  const user = await prisma.user.findUnique({
    where: { email: req.body.email },
  });

  if (!user || !(await bcrypt.compare(req.body.password, user.password))) {
    return res.status(401).json({ error: "Invalid credentials" });
  }

  const token = jwt.sign({ id: user.id }, "secret");
  res.json({ token });
});

// Protected route
app.get("/profile", auth, async (req, res) => {
  const user = await prisma.user.findUnique({
    where: { id: req.user.id },
  });
  res.json(user);
});

/* ---------- BACKGROUND JOB ---------- */
setInterval(() => {
  console.log("[NODE JOB] Background job running");
}, 5000);

/* ---------- WEBSOCKET ---------- */
io.on("connection", socket => {
  socket.emit("message", "Hello from Node WebSocket");
});

/* ---------- ERROR HANDLER ---------- */
app.use((err, req, res, next) => {
  res.status(500).json({ error: err.message });
});

/* ---------- START ---------- */
server.listen(3000, () => {
  console.log("🚀 Node server running on http://localhost:3000");
});
```

---

### **FILE 2 — Python (main.py)**

**Tech used:** FastAPI + SQLAlchemy + JWT + Pydantic + WebSocket

#### Install dependencies

```bash
pip install fastapi uvicorn sqlalchemy pydantic bcrypt pyjwt python-dotenv
```

---

###### **main.py (FULL WORKING CODE)**

```python
import jwt
import bcrypt
import threading
import time
from fastapi import FastAPI, Depends, HTTPException, WebSocket
from pydantic import BaseModel, EmailStr
from sqlalchemy import create_engine, Column, Integer, String
from sqlalchemy.orm import declarative_base, sessionmaker

# ---------- CONFIG ----------
SECRET = "secret"
engine = create_engine("sqlite:///db.sqlite")
Session = sessionmaker(bind=engine)
Base = declarative_base()

app = FastAPI()

# ---------- DATABASE ----------
class User(Base):
    __tablename__ = "users"
    id = Column(Integer, primary_key=True)
    email = Column(String, unique=True)
    password = Column(String)

Base.metadata.create_all(engine)

# ---------- SCHEMAS ----------
class UserCreate(BaseModel):
    email: EmailStr
    password: str

# ---------- DEPENDENCIES ----------
def get_db():
    db = Session()
    try:
        yield db
    finally:
        db.close()

def auth(token: str):
    try:
        return jwt.decode(token, SECRET, algorithms=["HS256"])
    except:
        raise HTTPException(status_code=401)

# ---------- ROUTES ----------
@app.get("/")
def home():
    return {"status": "Python API Running"}

@app.post("/register")
def register(user: UserCreate, db=Depends(get_db)):
    hashed = bcrypt.hashpw(user.password.encode(), bcrypt.gensalt())
    db.add(User(email=user.email, password=hashed.decode()))
    db.commit()
    return {"message": "User created"}

@app.post("/login")
def login(user: UserCreate, db=Depends(get_db)):
    u = db.query(User).filter(User.email == user.email).first()
    if not u or not bcrypt.checkpw(user.password.encode(), u.password.encode()):
        raise HTTPException(status_code=401)
    token = jwt.encode({"id": u.id}, SECRET, algorithm="HS256")
    return {"token": token}

@app.get("/profile")
def profile(token: str, db=Depends(get_db)):
    payload = auth(token)
    user = db.query(User).get(payload["id"])
    return {"id": user.id, "email": user.email}

# ---------- BACKGROUND JOB ----------
def job():
    while True:
        print("[PYTHON JOB] Background job running")
        time.sleep(5)

threading.Thread(target=job, daemon=True).start()

# ---------- WEBSOCKET ----------
@app.websocket("/ws")
async def ws(ws: WebSocket):
    await ws.accept()
    await ws.send_text("Hello from Python WebSocket")
```

Run with:

```bash
uvicorn main:app --reload
```

---

### **What this gives you**

| Feature         | Node       | Python      |
| --------------- | ---------- | ----------- |
| API server      | ✅         | ✅          |
| Routing         | ✅         | ✅          |
| Middleware / DI | ✅         | ✅          |
| Validation      | Zod        | Pydantic    |
| ORM             | Prisma     | SQLAlchemy  |
| JWT Auth        | ✅         | ✅          |
| Background Jobs | Native     | Thread      |
| WebSockets      | socket.io  | FastAPI WS  |
| Logging         | console    | print       |
| SQLite          | ✅         | ✅          |


# **Node.js + Express – Step by Step Setup**

**Step 1: Install Node.js**

* Download Node.js from [nodejs.org](https://nodejs.org) (LTS recommended)
* Or use a version manager like `nvm`:

```bash
nvm install node
nvm use node
```

**Step 2: Verify Installation**

```bash
node -v
npm -v
```

**Step 3:** Create project folder

```bash
mkdir node-auth-api
```

**Step 4:** Move into folder

```bash
cd node-auth-api
```

**Step 5:** Initialize Node project

```bash
npm init -y
```

**Step 6:** Install dependencies

```bash
npm install 
```

**Step 7:** Run server

```bash
node app.js
```

**Step 8:** Test APIs via Postman or curl:

* `POST /signup`
* `POST /login`
* `GET /profile` 



# **Python + FastAPI – Step by Step Setup**

**Step 1: Install Python**

* Download Python from [python.org](https://python.org) (Python 3.10+ recommended)
* Or use `pyenv` to manage multiple Python versions:

```bash
pyenv install 3.11.7
pyenv global 3.11.7
```

**Step 2: Verify Installation**

```bash
python --version
pip --version
```


**Step 3:** Create project folder

```bash
mkdir python-auth-api
```

**Step 4:** Move into folder

```bash
cd python-auth-api
```

**Step 5:** Create virtual environment

```bash
python -m venv venv
```

**Step 6:** Activate virtual environment

```bash
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

**Step 7:** Install dependencies

```bash
pip install -r requirements.txt
```

**Step 8:** Run FastAPI server

```bash
uvicorn app:app --reload --port 8000
```

**Step 9:** Test APIs via Postman or curl:

* `POST /signup`
* `POST /login`
* `GET /profile`