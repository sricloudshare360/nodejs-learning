
# Setup Node.js on Windows Laptop

This guide will walk you through installing and setting up Node.js on a Windows laptop.

## 1. Download Node.js Installer

- Visit the official Node.js website: [https://nodejs.org/](https://nodejs.org/)
- You’ll see two versions: 
  - **LTS (Long-Term Support)**: Recommended for most users (stable).
  - **Current**: Has the latest features but may not be as stable.
- Choose the appropriate version and download the Windows Installer (`.msi` file).

## 2. Install Node.js

- Open the downloaded `.msi` file.
- Follow the setup wizard:
  1. Accept the license agreement.
  2. Choose the installation path (default is recommended).
  3. Select components and ensure that "Add to PATH" is checked.
  4. Complete the installation.

## 3. Verify Node.js Installation

- Open Command Prompt (`cmd`) or PowerShell.
- Check if Node.js is installed correctly:

  ```bash
  node -v
  ```

- Check if `npm` (Node Package Manager) is installed:

  ```bash
  npm -v
  ```

## 4. Update npm (Optional)

- To update npm to the latest version, run:

  ```bash
  npm install -g npm@latest
  ```

## 5. Create a Simple Node.js Application

- Open a terminal and create a new directory:

  ```bash
  mkdir my-node-app
  cd my-node-app
  ```

- Create a file named `app.js`:

  ```bash
  echo console.log('Hello, Node.js!') > app.js
  ```

- Run the application:

  ```bash
  node app.js
  ```

- You should see the output:

  ```
  Hello, Node.js!
  ```

## 6. Install Packages Using npm

- You can use npm to install Node.js packages. For example, to install the `express` package:

  ```bash
  npm install express
  ```

- After installation, you can require it in your code:

  ```javascript
  const express = require('express');
  const app = express();
  ```

## 7. Troubleshooting

- If you encounter issues, ensure that:
  - The Node.js installation path is added to the `PATH` environment variable.
  - You restart the terminal after installation.
- If needed, reinstall Node.js using the installer.

## License

This guide is open-source and available under the MIT License.
