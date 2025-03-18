# first-demo
this is my first repository.
<br>
Author -- Vishakha Rathore.




// question no - 1 of assignment
let arr = [1, 2, 3, 4, 5];
let reversedarr=[]
for (let i = arr.length - 1; i >= 0; i--) {
    reversedarr.push(arr[i]); 
}
console.log(reversedarr);

// question no - 2
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
let evenSum = 0;
let oddSum = 0;

for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] % 2 === 0) {
        evenSum += numbers[i];  
    } else {
        oddSum += numbers[i];   
    }
}
let totalSum = evenSum + oddSum;
console.log("Sum of even numbers: " + evenSum);
console.log("Sum of odd numbers: " + oddSum);
console.log("Total sum (even + odd): " + totalSum);


// new assignment question 1

function calculateElectricityBill(units) {
  let billAmount = 0;

  // Calculate the bill based on units consumed
  if (units <= 100) {
    billAmount = units * 3;
  } else if (units <= 200) {
    billAmount = 100 * 3 + (units - 100) * 5;
  } else if (units <= 300) {
    billAmount = 100 * 3 + 100 * 5 + (units - 200) * 7;
  } else {
    billAmount = 100 * 3 + 100 * 5 + 100 * 7 + (units - 300) * 10;
  }

  // Apply 10% surcharge if bill exceeds ₹1000
  if (billAmount > 1000) {
    billAmount += billAmount * 0.10; // 10% surcharge
  }

  return billAmount;
}

// Example usage:
let unitsConsumed = 350;
let totalBill = calculateElectricityBill(unitsConsumed);
console.log("Total Electricity Bill: ₹" + totalBill);

// question 2
Task 1: Basic Loop Analysis
Code:
for(int i = 0; i < n; i++) {
    cout << "PhysicsWallah\n";
}

Time Complexity Analysis:

The loop runs from i = 0 to i < n, meaning it executes n times.
Each iteration prints "PhysicsWallah", which is a constant-time operation (O(1)).
Thus, the overall time complexity is determined by the number of iterations.
Conclusion:

The time complexity is O(n), as the loop runs n times.








