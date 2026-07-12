# JavaScript Interview Notes: Identifiers, Literals, and Null vs Undefined

## 1) Identifier in JavaScript

An identifier is the name given to variables, functions, classes, parameters, or labels.

### Important points
- Identifiers are used to refer to memory locations or program elements.
- They must follow naming rules.
- JavaScript identifiers are case-sensitive.
- Cannot start with a digit.
- Cannot use reserved keywords like `if`, `else`, `function`, `class`, etc.

### Valid examples
```javascript
let userName = "Alice";
let age = 25;
let _count = 1;
let $amount = 100;
```

### Invalid examples
```javascript
let 2name = "A";      // starts with a digit
let class = "Java";   // reserved keyword
let my-name = "A";    // hyphen is not allowed
```

### Interview tip
- A good identifier should be meaningful and readable.
- Example: `totalMarks` is better than `tm`.

---

## 2) Literal in JavaScript

A literal is a fixed value written directly in code.

### Common literals
- Number literal
```javascript
let age = 25;
```

- String literal
```javascript
let name = "John";
```

- Boolean literal
```javascript
let isActive = true;
```

- Object literal
```javascript
let person = { name: "John", age: 25 };
```

- Array literal
```javascript
let numbers = [1, 2, 3];
```

### Interview tip
- Literals represent fixed values.
- They are not variables or expressions; they are direct values in the source code.

---

## 3) Null vs Undefined

Both represent absence of value, but they are not the same.

### `undefined`
- A variable is declared but has not been assigned a value.
- A function parameter is missing.
- A function returns nothing explicitly.

```javascript
let x;
console.log(x); // undefined

function greet(name) {
  console.log(name);
}

greet(); // undefined
```

### `null`
- It is an intentional assignment meaning “no value” or “empty value”.
- It is usually used by developers to explicitly clear a value.

```javascript
let user = null;
console.log(user); // null
```

### Key difference
```javascript
let a;
console.log(a); // undefined

let b = null;
console.log(b); // null
```

### Interview points
- `undefined` means value is not assigned yet.
- `null` means the value is intentionally set to nothing.
- `typeof undefined` gives `"undefined"`.
- `typeof null` gives `"object"` in JavaScript (a classic interview point).

```javascript
console.log(typeof undefined); // "undefined"
console.log(typeof null); // "object"
```

---

## 4) Short Interview Summary

- Identifier = name of a variable/function/class.
- Literal = direct fixed value written in code.
- `undefined` = value not assigned yet.
- `null` = intentionally empty value.

## 5) One-line interview answer
- “An identifier is a name used to identify a program element, while a literal is a fixed value written directly in the code. `undefined` means a variable has no assigned value, whereas `null` means the value is intentionally set to no value.”
