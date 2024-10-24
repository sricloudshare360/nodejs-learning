
# Node.js Iteration App

This application demonstrates different iteration techniques in Node.js, including `for`, `for...of`, `for...in`, `while`, and `do...while` loops.

## Prerequisites

- Node.js (download from [nodejs.org](https://nodejs.org/))

## Getting Started

Follow these steps to create and run the application.

### 1. Clone the Repository

```bash
git clone <repository-url>
cd nodejs-iteration-app
```

### 2. Create `app.js`

Inside the project directory, create a file called `app.js` and add the following content:

```javascript
// app.js

function demonstrateIterations() {
    const array = [1, 2, 3, 4, 5];
    const object = { a: 1, b: 2, c: 3 };

    console.log('=== For Loop ===');
    for (let i = 0; i < array.length; i++) {
        console.log(\`Index \${i}: \${array[i]}\`);
    }

    console.log('\n=== For...of Loop ===');
    for (const value of array) {
        console.log(\`Value: \${value}\`);
    }

    console.log('\n=== For...in Loop (Object) ===');
    for (const key in object) {
        if (object.hasOwnProperty(key)) {
            console.log(\`Key: \${key}, Value: \${object[key]}\`);
        }
    }

    console.log('\n=== For...in Loop (Array) ===');
    for (const index in array) {
        console.log(\`Index \${index}: \${array[index]}\`);
    }

    console.log('\n=== While Loop ===');
    let i = 0;
    while (i < array.length) {
        console.log(\`Index \${i}: \${array[i]}\`);
        i++;
    }

    console.log('\n=== Do...While Loop ===');
    i = 0;
    do {
        console.log(\`Index \${i}: \${array[i]}\`);
        i++;
    } while (i < array.length);
}

// Call the function to demonstrate iterations
demonstrateIterations();
```

### 3. Run the Application

Run the application using Node.js:

```bash
node app.js
```

### Expected Output

```
=== For Loop ===
Index 0: 1
Index 1: 2
Index 2: 3
Index 3: 4
Index 4: 5

=== For...of Loop ===
Value: 1
Value: 2
Value: 3
Value: 4
Value: 5

=== For...in Loop (Object) ===
Key: a, Value: 1
Key: b, Value: 2
Key: c, Value: 3

=== For...in Loop (Array) ===
Index 0: 1
Index 1: 2
Index 2: 3
Index 3: 4
Index 4: 5

=== While Loop ===
Index 0: 1
Index 1: 2
Index 2: 3
Index 3: 4
Index 4: 5

=== Do...While Loop ===
Index 0: 1
Index 1: 2
Index 2: 3
Index 3: 4
Index 4: 5
```

## License

This project is licensed under the MIT License.
