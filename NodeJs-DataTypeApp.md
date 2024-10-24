
# Node.js Data Type App

This application demonstrates how to identify and handle different data types in Node.js, including strings, numbers, booleans, arrays, objects, null, and undefined.

## Prerequisites

- Node.js (download from [nodejs.org](https://nodejs.org/))

## Getting Started

Follow these steps to create and run the application.

### 1. Clone the Repository

```bash
git clone <repository-url>
cd nodejs-data-type-app
```

### 2. Create `app.js`

Inside the project directory, create a file called `app.js` and add the following content:

```javascript
// app.js

function identifyDataType(input) {
    if (typeof input === 'string') {
        console.log(\`Data Type: String, Value: "\${input}"\`);
    } else if (typeof input === 'number') {
        console.log(\`Data Type: Number, Value: \${input}\`);
    } else if (typeof input === 'boolean') {
        console.log(\`Data Type: Boolean, Value: \${input}\`);
    } else if (Array.isArray(input)) {
        console.log(\`Data Type: Array, Values: [\${input.join(', ')}]\`);
    } else if (typeof input === 'object' && input !== null) {
        console.log(\`Data Type: Object, Value: \${JSON.stringify(input)}\`);
    } else if (input === null) {
        console.log('Data Type: Null, Value: null');
    } else if (typeof input === 'undefined') {
        console.log('Data Type: Undefined');
    } else {
        console.log('Data Type: Unknown');
    }
}

// Examples
identifyDataType('Hello, World!');
identifyDataType(42);
identifyDataType(true);
identifyDataType([1, 2, 3, 4]);
identifyDataType({ name: 'Alice', age: 25 });
identifyDataType(null);
identifyDataType(undefined);
```

### 3. Run the Application

Run the application using Node.js:

```bash
node app.js
```

### Expected Output

```
Data Type: String, Value: "Hello, World!"
Data Type: Number, Value: 42
Data Type: Boolean, Value: true
Data Type: Array, Values: [1, 2, 3, 4]
Data Type: Object, Value: {"name":"Alice","age":25}
Data Type: Null, Value: null
Data Type: Undefined
```

## License

This project is licensed under the MIT License.
