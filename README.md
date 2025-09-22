# Constructors_Deconstructors_cpp

# Constructors in C++

A **constructor** in C++ is a special member function that is automatically executed whenever an object of a class is created. Its primary role is to **initialize the data members** of the object, ensuring that it begins in a valid and well-defined state.

---

## Key Features of Constructors

- The constructor’s **name must match the class name**.
- It **has no return type** (not even `void`).
- It is **automatically called** when an object is created.
- Constructors can be **overloaded** (multiple constructors with different parameters).
- If no constructor is defined, the **compiler supplies a default constructor**.

## Types of Constructors

### 1. Default Constructor
- Takes **no arguments**.
- Initializes objects with **default or pre-defined values**.

### 2. Parameterized Constructor
- Accepts **arguments** to initialize objects with **user-specified values**.
- Provides **flexibility** at the time of object creation.

### 3. Copy Constructor
- Creates a **new object** as a copy of an existing object.
- **Syntax:**
```cpp
ClassName(const ClassName &obj) { 
    // copy member variables from obj
}

## Copy Constructor Usage

- Commonly used in cases like:
  - Passing objects by value
  - Returning objects from functions
  - Duplicating existing objects

---

## Advantages of Constructors

- Ensure **automatic and consistent initialization**.
- Improve **readability** and reduce redundant initialization code.
- Support **polymorphism** via overloading.

---

## Limitations of Constructors

- Cannot be **virtual**.
- Cannot **return values**.
- Cannot be **inherited**, though base class constructors can be invoked in derived classes using **initializer lists**.
- Cannot be **explicitly invoked** like normal functions (only called through object creation).

---

# Destructors in C++

A **destructor** is a special member function automatically invoked when an object goes out of scope or is explicitly deleted. Its purpose is to **release resources** acquired during the object’s lifetime, such as memory, file handles, or network connections.

---

## Key Features of Destructors

- Same name as the class, but preceded by a **tilde `~`**.
- Takes **no arguments** and has **no return type**.
- Only **one destructor** is allowed per class (cannot be overloaded).
- Invoked automatically in **reverse order of object creation**.

---

## Uses of Destructors

- Free **dynamically allocated memory**.
- Close **files** or **network connections**.
- Release **system resources** like locks.
- Debugging/logging **object lifecycle**.

---

## Advantages of Destructors

- Automatic **cleanup of resources**.
- Prevents **memory leaks**.
- Simplifies code by embedding **cleanup logic** inside the class.
- Improves program **stability** by handling resource deallocation.

---

## Limitations of Destructors

- Called in **reverse order of construction** in inheritance chains.
- Cannot be **overloaded**.
- Order of destructor calls for **global/static objects across files** is undefined.
- Should **not throw exceptions** (unsafe).
