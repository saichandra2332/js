# js
function reverseNumber(num) {
  let reversed = 0;
  
  while (num > 0) {
    const digit = num % 10; // get the last digit of the number
    reversed = (reversed * 10) + digit; // add the digit to the reversed number
    num = Math.floor(num / 10); // remove the last digit from the original number
  }
  
  return reversed;
}

// Example usage
console.log(reverseNumber(123)); // Output: 321
console.log(reverseNumber(9876)); // Output: 6789
console.log(reverseNumber(100)); // Output: 1
