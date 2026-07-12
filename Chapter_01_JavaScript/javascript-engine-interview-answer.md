# Short Interview Answer: How JavaScript Engine Works

A JavaScript engine is the program that runs JavaScript code inside the browser or Node.js. First, it parses the code and creates an Abstract Syntax Tree (AST), which helps it understand the structure of the program. Then it compiles the code into machine-readable instructions, often using Just-In-Time (JIT) compilation for better performance.

The engine also manages memory by using the call stack for executing functions and the heap for storing objects and dynamic data. It keeps track of variable scopes, handles function calls, and uses a garbage collector to remove unused memory automatically. In simple terms, the JavaScript engine works like a translator and executor that turns human-written code into fast, efficient runtime behavior.

Example:

```javascript
function greet(name) {
  return "Hello, " + name;
}

console.log(greet("Alice"));
```

When this code runs, the engine parses it, creates the function, stores it in memory, and then executes it step by step. The call stack handles the function call, and the engine manages the result so it can be displayed in the console.
