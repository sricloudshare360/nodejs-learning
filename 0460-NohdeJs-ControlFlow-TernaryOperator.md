function isAdult(age) {
  const status = age >= 18 ? "Adult" : "Minor";
  console.log(status);
}

isAdult(20); // Output: Adult
isAdult(15); // Output: Minor
