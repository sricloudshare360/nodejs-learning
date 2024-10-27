
# Node.js Function App

This application demonstrates the use of functions in Node.js, including basic functions, functions with parameters, arrow functions, functions with return values, and functions with callbacks.

## Prerequisites

- Node.js (download from [nodejs.org](https://nodejs.org/))

## Getting Started

Follow these steps to create and run the application.

### 1. Clone the Repository

```bash
git clone <repository-url>
cd nodejs-function-app
```

### 2. Create `app.js`

Inside the project directory, create a file called `app.js` and add the following content:

```javascript
// app.js

// Basic function
function greet() {
    console.log('Hello, World!');
}

// Function with parameters
function add(a, b) {
    return a + b;
}

// Arrow function
const multiply = (a, b) => a * b;

// Function with a callback
function fetchData(callback) {
    setTimeout(() => {
        const data = { name: 'Alice', age: 25 };
        callback(data);
    }, 1000);
}

// Function with parameters and return value
function introduce(name, age) {
    return \`My name is \${name} and I am \${age} years old.\`;
}

// Call the functions
greet();
console.log(\`Addition: \${add(2, 3)}\`);
console.log(\`Multiplication: \${multiply(4, 5)}\`);

fetchData((data) => {
    console.log(\`Fetched Data: \${JSON.stringify(data)}\`);
});

console.log(introduce('Bob', 30));
```

### 3. Run the Application

Run the application using Node.js:

```bash
node app.js
```

### Expected Output

```
Hello, World!
Addition: 5
Multiplication: 20
Fetched Data: {"name":"Alice","age":25}
My name is Bob and I am 30 years old.
```

## Explanation of Function Types

- **Basic Function**: A simple function that performs a specific task.
- **Function with Parameters**: Takes inputs (parameters) to perform calculations or operations.
- **Arrow Function**: A shorter syntax for writing functions in JavaScript.
- **Callback Function**: A function passed as an argument to another function and executed after some operation is completed.
- **Function with Return Value**: Returns a value to the calling function.

## License

This project is licensed under the MIT License.
