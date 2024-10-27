function divide(a, b) {
  try {
    if (b === 0) {
      throw new Error("Division by zero");
    }
    console.log(a / b);
  } catch (error) {
    console.error(error.message);
  } finally {
    console.log("Execution complete.");
  }
}

divide(10, 2); // Output: 5  Execution complete.
divide(5, 0);  // Output: Division by zero  Execution complete.