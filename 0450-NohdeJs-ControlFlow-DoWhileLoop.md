function printAtLeastOnce(number) {
  do {
    console.log(number);
    number--;
  } while (number > 0);
}

printAtLeastOnce(0); // Output: 0 (executes at least once even if condition is false)